<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Free Robux, V-Bucks & Minecoins Generator</title>
  <style>
    body {
      background: linear-gradient(135deg, #1a1a1a, #0f0f0f);
      color: #ffffff;
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      text-align: center;
    }
    h1 {
      font-size: 2.7em;
      color: #00ffcc;
      margin-bottom: 10px;
    }
    p {
      font-size: 1.2em;
      color: #dddddd;
    }
    input {
      padding: 12px;
      font-size: 16px;
      width: 280px;
      margin-top: 20px;
      border: none;
      border-radius: 10px;
      outline: none;
    }
    button {
      margin-top: 25px;
      padding: 14px 30px;
      font-size: 18px;
      background: #1db954;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover {
      background: #17a44c;
    }
    #progressContainer {
      width: 80%;
      background: #333;
      border-radius: 15px;
      margin-top: 30px;
      height: 25px;
      overflow: hidden;
      display: none;
    }
    #progressBar {
      height: 100%;
      width: 0%;
      background: #00ffcc;
      transition: width 0.1s ease-in-out;
    }
    .footer {
      position: absolute;
      bottom: 15px;
      font-size: 0.9em;
      color: #666;
    }
  </style>
</head>
<body>
  <h1>💰 Get Free Robux, V-Bucks & Minecoins 💎</h1>
  <p>Enter your <strong>Roblox, Fortnite or Minecraft</strong> username:</p>
  <input type="text" id="username" placeholder="Enter your username" />
  <br>
  <button onclick="startFakeHack()">Generate Now</button>

  <div id="progressContainer">
    <div id="progressBar"></div>
  </div>

  <div class="footer">© 2025 LootDrop™ | For entertainment only 😎</div>

  <script>
    function startFakeHack() {
      const username = document.getElementById('username').value.trim();
      if (!username) {
        alert("Bruhh... enter your username first 😅");
        return;
      }

      document.getElementById('progressContainer').style.display = 'block';
      let progress = 0;
      let bar = document.getElementById('progressBar');
      let fakeLoading = setInterval(() => {
        progress += Math.random() * 5; // Make it kinda random
        bar.style.width = progress + "%";
        if (progress >= 100) {
          clearInterval(fakeLoading);
          setTimeout(() => {
            window.location.href = "https://www.youtube.com/watch?v=dQw4w9WgXcQ";
          }, 500);
        }
      }, 100);
    }
  </script>
</body>
</html>
