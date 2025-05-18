<!DOCTYPE html>
<html lang="zh-TW">
<head>
  <meta charset="UTF-8">
  <title>ISCG-ESport</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    html, body {
      margin: 0;
      padding: 0;
      width: 100vw;
      height: 100vh;
      overflow: hidden;
      font-family: 'Orbitron', sans-serif;
      background-color: #000;
      color: white;
    }
    #login-container {
      width: 100vw;
      height: 100vh;
      background: radial-gradient(circle at center, #1a1a1a, #000);
      border: 5px solid #e60073;
      box-shadow: 0 0 40px #e60073;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
    #login-box {
      background: rgba(0, 0, 0, 0.85);
      padding: 30px;
      border-radius: 12px;
      text-align: center;
      max-width: 90%;
    }
    #login-box img {
      width: 120px;
      height: auto;
      margin-bottom: 20px;
    }
    #login-box input {
      padding: 10px;
      border-radius: 5px;
      border: none;
      width: 80%;
      margin: 10px 0;
      font-size: 1em;
    }
    #login-box button {
      padding: 10px 20px;
      background-color: #e60073;
      border: none;
      color: white;
      font-weight: bold;
      border-radius: 5px;
      cursor: pointer;
    }
    #main-interface {
      display: none;
      width: 100vw;
      height: 100vh;
      padding: 20px;
      box-sizing: border-box;
      background: linear-gradient(135deg, #111, #000);
      overflow-y: auto;
    }
    .announcement, .sponsor-list {
      background: rgba(255, 255, 255, 0.1);
      border-left: 5px solid #e60073;
      padding: 20px;
      margin-bottom: 20px;
      border-radius: 10px;
    }
    h2 {
      color: #e60073;
      margin-bottom: 10px;
    }
    ul {
      list-style-type: none;
      padding-left: 0;
    }
    li::before {
      content: "★ ";
      color: #ff007f;
    }
  </style>
</head>
<body>
  <!-- 登入畫面 -->
  <div id="login-container">
    <div id="login-box">
      <img src="IMG_20250413_172657_723.webp" alt="ISCG Logo">
      <h1>ISCG E<sup>Sport</sup></h1>
      <p>請輸入戰隊專屬密碼以檢視群組資訊：</p>
      <input type="password" id="password" placeholder="請輸入密碼">
      <br>
      <button onclick="verifyPassword()">確認</button>
    </div>
  </div>
  <!-- 主畫面 -->
  <div id="main-interface">
    <div class="announcement">
      <h2>戰隊公告：</h2>
      <p>（公告內容...）</p>
    </div>
    <div class="sponsor-list">
      <h2>贊助名單（50鑽凝膠護盾）</h2>
      <ul>
        <li>玩家A</li>
        <li>玩家B</li>
        <li>玩家C</li>
        <!-- 可自行新增 -->
      </ul>
    </div>
  </div>
  <script>
    function verifyPassword() {
      const input = document.getElementById("password").value;
      const correctPassword = "0809"; // 可自訂密碼
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
