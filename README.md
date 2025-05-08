// animated-profile.ts
import chalk from 'chalk';
import chalkAnimation from 'chalk-animation';
import figlet from 'figlet';
import { setTimeout } from 'timers/promises';

interface Profile {
  name: string;
  age: number;
  gender: string;
  skills: string[];
  rating: number;
  note: string;
}

const profile: Profile = {
  name: '天音さら',
  age: 19,
  gender: '女性',
  skills: [
    'Java / Kotlin (メイン)',
    'Python',
    'JavaScript / TypeScript',
    'C++ / C# / C',
    'HTML & CSS',
  ],
  rating: 1900,
  note: 'ソースコードを公開していきます！',
};

async function animateHeader(text: string) {
  // レインボーアニメーションで大見出し
  const animation = chalkAnimation.rainbow(figlet.textSync(text, {
    horizontalLayout: 'full',
    verticalLayout: 'default',
  }));
  // 2秒間アニメーション表示
  await setTimeout(2000);
  animation.stop();
}

function printProfile(p: Profile) {
  console.log(chalk.bold.hex('#FF69B4')('☆ プロフィール ☆'));
  console.log(`${chalk.bold.cyan('👤 名前:')} ${chalk.white(p.name)}`);
  console.log(`${chalk.bold.cyan('🎂 年齢:')} ${chalk.white(`${p.age}歳`)}`);
  console.log(`${chalk.bold.cyan('🚻 性別:')} ${chalk.white(p.gender)}`);
  console.log(chalk.bold.magenta('💻 スキルセット:'));
  p.skills.forEach((s) =>
    console.log(`  ${chalk.green('•')} ${chalk.white(s)}`)
  );
  console.log(
    `${chalk.bold.yellow('🥇 AtCoder Rating:')} ${chalk.white(p.rating)}`
  );
  console.log(`${chalk.bold.gray('🤖')} ${chalk.white(p.note)}`);
}

async function main() {
  await animateHeader('Sara Amane');  
  printProfile(profile);
  console.log(chalk.italic.dim('— ご依頼・コラボ歓迎！'));
}

main();
