<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>deax プロフィール</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: #fff5fa;
    }

    .profile-container {
      font-family: "Segoe UI", sans-serif;
      background: linear-gradient(145deg, #ffe4ec, #ffe0f0);
      border-radius: 20px;
      padding: 2rem;
      max-width: 960px;
      margin: 2rem auto;
      box-shadow: 0 10px 30px rgba(255, 182, 193, 0.4);
    }

    .badge-list {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      justify-content: center;
      margin-bottom: 2rem;
    }

    .badge {
      border-radius: 12px;
      overflow: hidden;
      padding: 3px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
      background: #fff0f5;
      transition: transform 0.2s ease-in-out;
    }

    .badge:hover {
      transform: scale(1.08);
    }

    .profile-card {
      text-align: center;
      background: white;
      padding: 2rem;
      border-radius: 16px;
      border: 2px dashed #ffb6c1;
      box-shadow: 0 5px 15px rgba(255, 182, 193, 0.3);
    }

    .profile-card h1 {
      font-size: 2.5rem;
      color: #d63384;
      margin-bottom: 1rem;
    }

    .profile-card p {
      font-size: 1.25rem;
      margin: 0.5rem 0;
      color: #555;
    }

    .github-stats {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 1rem;
      margin-top: 1.5rem;
    }

    .links p {
      margin: 0.5rem 0;
      font-size: 1.1rem;
    }

    .links a {
      color: #e83e8c;
      text-decoration: none;
      font-weight: bold;
    }

    .links a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <!-- モダンでピンク可愛いバッジ群 + プロフィールUI -->
  <div class="profile-container">
    <div class="badge-list">
      <span class="badge"><img src="https://img.shields.io/badge/Java-F89820?style=flat&logo=java&logoColor=white" alt="Java"></span>
      <span class="badge"><img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white" alt="Kotlin"></span>
      <span class="badge"><img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python"></span>
      <span class="badge"><img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black" alt="JavaScript"></span>
      <span class="badge"><img src="https://img.shields.io/badge/C++-00599C?style=flat&logo=c%2B%2B&logoColor=white" alt="C++"></span>
      <span class="badge"><img src="https://img.shields.io/badge/C%23-92008D?style=flat&logo=c-sharp&logoColor=white" alt="C#"></span>
      <span class="badge"><img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white" alt="HTML5"></span>
      <span class="badge"><img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white" alt="CSS3"></span>
    </div>

    <div class="profile-card">
      <h1>👋 こんにちは！ deaxです。</h1>
      <p><strong>🧑‍🎓 19歳女 ・ AtCoder総合レーティング 2140</strong></p>
      <div class="github-stats">
        <img src="https://github-readme-stats.vercel.app/api?username=deaxcode&show_icons=true&theme=radical&hide_border=true&count_private=true" alt="GitHub Stats">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=deaxcode&layout=compact&theme=radical&hide_border=true" alt="Top Langs">
      </div>
      <div class="links">
        <p>🌐 <a href="https://voidcore.jp">https://voidcore.jp</a></p>
        <p>💬 <a href="https://discord.gg/voidcore">discord.gg/voidcore</a></p>
      </div>
    </div>
  </div>
</body>
</html>
