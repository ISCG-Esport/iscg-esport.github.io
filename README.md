<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ISCG ᴱSport 戰隊資訊頁</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #0f0f0f, #1a1a1a);
      color: #f0f0f0;
      text-align: center;
      padding: 2rem;
      margin: 0;
    }
    .container {
      max-width: 700px;
      margin: 0 auto;
      background: #111;
      border-radius: 20px;
      padding: 2rem;
      box-shadow: 0 0 30px rgba(255, 0, 85, 0.4);
      transition: all 0.3s ease;
    }
    input[type="password"] {
      padding: 0.7rem;
      width: 60%;
      font-size: 1rem;
      border-radius: 8px;
      border: none;
      margin-bottom: 1rem;
      background: #222;
      color: #fff;
    }
    button {
      background-color: #ff0055;
      color: white;
      padding: 0.6rem 1.2rem;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    button:hover {
      background-color: #ff3366;
    }
    .links {
      margin-top: 2rem;
    }
    .links a {
      display: block;
      background: #222;
      color: #00ccff;
      margin: 0.5rem 0;
      padding: 0.8rem;
      border-radius: 10px;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s ease;
    }
    .links a:hover {
      background: #333;
    }
    .announcement {
      background-color: #1f1f1f;
      padding: 1rem;
      border-radius: 10px;
      margin-bottom: 1.5rem;
      border-left: 5px solid #ff0055;
      text-align: left;
    }
  </style>
</head>
<body>
  <div class="container" id="loginContainer">
    <h1>ISCG ᴱSport</h1>
    <p>請輸入戰隊專屬密碼以檢視群組資訊：</p>
    <input type="password" id="password" placeholder="請輸入密碼">
    <br>
    <button onclick="checkPassword()">確認</button>
  </div>  <div class="container" id="contentContainer" style="display: none;">
    <div class="announcement">
      <strong>戰隊公告：</strong>
      <p>（請在此輸入戰隊公告內容）</p>
    </div>
    <div class="links">
      <h2>戰隊群組連結</h2>
      <a href="https://discord.gg/fanQdSv4PK" target="_blank">⚠️ Discord 戰隊群</a>
      <a href="https://vt.tiktok.com/ZSHXGFkaU48Jg-cZ9XU/" target="_blank">⚠️ TikTok 戰隊群</a>
      <a href="https://ig.me/j/AbbADUNsweizIrmP/" target="_blank">⚠️ IG 戰隊群</a>
    </div>
  </div>  <script>
    function checkPassword() {
      const input = document.getElementById('password').value;
      const correctPassword = '0809';
      if (input === correctPassword) {
        document.getElementById('loginContainer').style.display = 'none';
        document.getElementById('contentContainer').style.display = 'block';
      } else {
        alert('密碼錯誤，請重新輸入');
      }
    }
  </script></body>
