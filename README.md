<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ISCG ᴱSport 戰隊入口</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #000;
      color: #fff;
    }
    header {
      text-align: center;
      font-size: 2rem;
      padding: 20px;
      color: #2aa0ff;
    }
    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      background: radial-gradient(circle, #1b1b1b 30%, #000000 100%);
      box-shadow: 0 0 30px #f40076;
    }
    .login-box {
      background-color: rgba(0, 0, 0, 0.8);
      padding: 40px;
      border-radius: 12px;
      text-align: center;
      width: 90%;
      max-width: 500px;
    }
    .login-box h2 {
      margin-bottom: 20px;
    }
    input[type="password"] {
      width: 80%;
      padding: 10px;
      font-size: 1rem;
      border-radius: 6px;
      border: none;
    }
    button {
      margin-top: 15px;
      padding: 10px 20px;
      background-color: #f40076;
      border: none;
      color: white;
      font-size: 1rem;
      border-radius: 6px;
      cursor: pointer;
    }
    .content {
      display: none;
      padding: 20px;
    }
    .announcement {
      background-color: #111;
      padding: 15px;
      border-left: 4px solid #2aa0ff;
      margin-bottom: 20px;
    }
    .link-box {
      margin: 10px 0;
      background-color: #1e1e1e;
      padding: 10px;
      border-radius: 8px;
      display: flex;
      align-items: center;
    }
    .link-box img {
      width: 24px;
      height: 24px;
      margin-right: 10px;
    }
    .link-box a {
      color: #fff;
      text-decoration: none;
    }
    .logo {
      width: 80px;
      margin-bottom: 20px;
    }
  </style>
</head>
<body>
  <header>ISCG-Esport</header>
  <div class="container" id="login-container">
    <div class="login-box">
      <img src="https://img.icons8.com/?size=48&id=30998&format=png" class="logo" alt="戰隊標誌">
      <h2>ISCG ᴱSport</h2>
      <p>請輸入戰隊專屬密碼以檢視群組資訊：</p>
      <input type="password" id="password" placeholder="請輸入密碼" />
      <br />
      <button onclick="checkPassword()">確認</button>
    </div>
  </div>  <div class="content" id="content">
    <div class="announcement">
      <strong>戰隊公告：</strong>
      <p>（請在此填寫公告內容）</p>
    </div>
    <div class="link-box">
      <img src="https://img.icons8.com/?size=48&id=30998&format=png" alt="Discord">
      <a href="https://discord.gg/fanQdSv4PK" target="_blank">Discord 戰隊群</a>
    </div>
    <div class="link-box">
      <img src="https://img.icons8.com/?size=48&id=118497&format=png" alt="TikTok">
      <a href="https://vt.tiktok.com/ZSHXGFkaU48Jg-cZ9XU/" target="_blank">TikTok 戰隊群</a>
    </div>
    <div class="link-box">
      <img src="https://img.icons8.com/?size=48&id=32292&format=png" alt="Instagram">
      <a href="https://ig.me/j/AbbADUNsweizIrmP/" target="_blank">Instagram 戰隊群</a>
    </div>
  </div>  <script>
    function checkPassword() {
      const correctPassword = "0809";
      const input = document.getElementById("password").value;
      if (input === correctPassword) {
        document.getElementById("login-container").style.display = "none";
        document.getElementById("content").style.display = "block";
      } else {
        alert("密碼錯誤，請再試一次。");
      }
    }
  </script></body>
