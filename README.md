<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ISCG E-Sport 登入</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Orbitron', sans-serif;
      background: linear-gradient(135deg, #0f0f0f, #1c1c1c);
      color: #ffffff;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
    }
    .container {
      background: radial-gradient(circle at center, #1b1b1b, #0f0f0f);
      border: 2px solid #ff0055;
      border-radius: 20px;
      padding: 40px;
      box-shadow: 0 0 40px rgba(255, 0, 85, 0.7);
      width: 90%;
      max-width: 400px;
      text-align: center;
    }
    .logo {
      width: 120px;
      height: 120px;
      object-fit: cover;
      border-radius: 50%;
      margin-bottom: 20px;
      box-shadow: 0 0 20px rgba(255, 0, 85, 0.7);
    }
    h1 {
      margin-bottom: 10px;
      font-size: 28px;
      color: #ff0055;
    }
    input[type="password"] {
      width: 100%;
      padding: 10px;
      margin: 15px 0;
      font-size: 16px;
      border: none;
      border-radius: 10px;
    }
    button {
      background-color: #ff0055;
      color: white;
      padding: 12px 30px;
      border: none;
      border-radius: 10px;
      font-size: 16px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    button:hover {
      background-color: #cc0044;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <div class="container" id="login">
    <img src="IMG_20250413_172657_723.webp" alt="ISCG Logo" class="logo">
    <h1>ISCG E-Sport</h1>
    <p>請輸入戰隊專屬密碼以檢視群組資訊：</p>
    <input type="password" id="password" placeholder="請輸入密碼">
    <button onclick="checkPassword()">確認</button>
  </div>

  <div class="container hidden" id="content">
    <h1>戰隊公告：</h1>
    <div style="background:#111; border-left: 4px solid #ff0055; padding: 15px; margin-bottom: 20px; border-radius: 8px;">
      請在此自行填入公告內容。
    </div>
    <p><img src="https://cdn-icons-png.flaticon.com/512/3670/3670157.png" style="width:20px; vertical-align:middle;"> <a href="https://discord.gg/fanQdSv4PK" style="color:#fff;">DC戰隊群連結</a></p>
    <p><img src="https://cdn-icons-png.flaticon.com/512/3046/3046121.png" style="width:20px; vertical-align:middle;"> <a href="https://vt.tiktok.com/ZSHXGFkaU48Jg-cZ9XU/" style="color:#fff;">Tiktok戰隊群連結</a></p>
    <p><img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" style="width:20px; vertical-align:middle;"> <a href="https://ig.me/j/AbbADUNsweizIrmP/" style="color:#fff;">IG戰隊群連結</a></p>
  </div>

  <script>
    function checkPassword() {
      const pwd = document.getElementById('password').value;
      if (pwd === '0809') {
        document.getElementById('login').classList.add('hidden');
        document.getElementById('content').classList.remove('hidden');
      } else {
        alert('密碼錯誤！');
      }
    }
  </script>
</body>
