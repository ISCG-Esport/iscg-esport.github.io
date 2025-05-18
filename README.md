<!DOCTYPE html>
<html lang="zh-TW">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ISCG-Esport</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      width: 100vw;
      height: 100vh;
      background: #000;
      font-family: 'Orbitron', sans-serif;
      color: #fff;
      overflow: hidden;
    }
    #login-container {
      width: 100vw;
      height: 100vh;
      box-sizing: border-box;
      border: 6px solid #ff007f;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }
    #login-box {
      background-color: rgba(0, 0, 0, 0.9);
      border-radius: 20px;
      padding: 30px;
      width: 90%;
      max-width: 400px;
      text-align: center;
      box-shadow: 0 0 20px #ff007f;
    }
    #login-box img {
      width: 160px;
      margin-bottom: 20px;
    }
    h1 {
      font-size: 2em;
      color: #ff007f;
      margin-bottom: 10px;
    }
    p {
      margin: 10px 0;
      font-size: 1rem;
    }
    input {
      width: 90%;
      padding: 12px;
      font-size: 1rem;
      margin-top: 10px;
      border-radius: 5px;
      border: none;
    }
    button {
      margin-top: 15px;
      padding: 10px 25px;
      font-size: 1rem;
      font-weight: bold;
      background-color: #ff007f;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    #main-interface {
      display: none;
      width: 100vw;
      height: 100vh;
      background-color: #000;
      color: white;
      padding: 20px;
      box-sizing: border-box;
      overflow-y: auto;
    }
    .announcement, .sponsor-list, .group-links {
      margin-bottom: 20px;
      padding: 20px;
      background: rgba(255,255,255,0.08);
      border-left: 5px solid #ff007f;
      border-radius: 12px;
    }
    h2 {
      color: #ff007f;
      margin-bottom: 10px;
    }
    ul {
      list-style: none;
      padding: 0;
    }
    li::before {
      content: "★ ";
      color: #ff007f;
    }
    a {
      color: #00ffff;
      text-decoration: underline;
    }

  </style>
</head>
<body>

  <!-- 登入畫面 -->
  <div id="login-container">
    <div id="login-box">
      <img src="IMG_20250413_172657_723.webp" alt="Logo">
      <h1>ISCG E<sup>Sport</sup></h1>
      <p>請輸入戰隊專屬密碼以檢視群組資訊：</p>
      <input type="password" id="password" placeholder="請輸入 密碼">
      <br>
      <button onclick="verifyPassword()">確認</button>
    </div>
  </div>

  <!-- 主畫面內容 -->
  <div id="main-interface">
    <div class="announcement">
      <h2>戰隊公告</h2>
      <p>公告...</p>
    </div>
    <div class="group-links">
      <h2>戰隊群組連結</h2>
      <ul>
<div class="link-box">
      <img src="https://img.icons8.com/?size=48&id=30998&format=png" alt="Discord">
      <a href="https://discord.gg/fanQdSv4PK" target="_blank">Discord 戰隊群</a>
    </div>
    <div class="link-box">
      <img src="https://images.app.goo.gl/eNzNS" alt="TikTok">
      <a href="https://vt.tiktok.com/ZSHXGFkaU48Jg-cZ9XU/" target="_blank">TikTok 戰隊群</a>
    </div>
    <div class="link-box">
      <img src="https://img.icons8.com/?size=48&id=32292&format=png" alt="Instagram">
      <a href="https://ig.me/j/AbbADUNsweizIrmP/" target="_blank">Instagram 戰隊群</a>
    </div>
  <div class="sponsor-list">
      <h2>贊助名單（50鑽凝膠）</h2>
      <ul>
        <li>玩家A</li>
        <li>玩家B</li>
        <li>玩家C</li>
      </ul>
    </div>
  </div>

  <script>
    function verifyPassword() {
      const input = document.getElementById("password").value;
      const correctPassword = "0809"; // 你可以自行修改

      if (input === correctPassword) {
        document.getElementById("login-container").style.display = "none";
        document.getElementById("main-interface").style.display = "block";
      } else {
        alert("密碼錯誤，請再試一次！");
      }
    }
  </script>
</body>
</html>
