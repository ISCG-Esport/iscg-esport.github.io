<!DOCTYPE html><html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ISCG ᴱSport 戰隊資訊頁</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #0d0d0d;
      color: white;
      text-align: center;
      padding: 2rem;
    }
    .container {
      max-width: 600px;
      margin: 0 auto;
      background: #1a1a1a;
      border-radius: 15px;
      padding: 2rem;
      box-shadow: 0 0 20px rgba(255, 0, 85, 0.4);
    }
    input[type="password"] {
      padding: 0.5rem;
      width: 60%;
      font-size: 1rem;
      border-radius: 5px;
      border: none;
      margin-bottom: 1rem;
    }
    button {
      background-color: #ff0055;
      color: white;
      padding: 0.5rem 1rem;
      border: none;
      border-radius: 5px;
      font-size: 1rem;
      cursor: pointer;
    }
    .links {
      margin-top: 2rem;
    }
    .links a {
      display: block;
      color: #00ccff;
      margin: 0.5rem 0;
      text-decoration: none;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>ISCG ᴱSport</h1>
    <p>請輸入戰隊專屬密碼以檢視群組資訊：</p>
    <input type="password" id="password" placeholder="請輸入密碼">
    <br>
    <button onclick="checkPassword()">確認</button><div class="links" id="links" style="display: none;">
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
        document.getElementById('links').style.display = 'block';
      } else {
        alert('密碼錯誤，請重新輸入');
      }
    }
  </script></body>
</html>
