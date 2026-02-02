<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Be My Valentine 💖</title>

  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #ff9a9e, #fecfef);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Comic Sans MS', cursive;
      overflow: hidden;
    }

    .container {
      text-align: center;
      background: rgba(255, 255, 255, 0.9);
      padding: 40px;
      border-radius: 25px;
      box-shadow: 0 15px 40px rgba(0,0,0,0.25);
      max-width: 400px;
    }

    h1 {
      color: #ff3366;
      margin-bottom: 25px;
    }

    button {
      font-size: 20px;
      padding: 12px 28px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
    }

    #yesBtn {
      background-color: #ff3366;
      color: white;
      margin-right: 20px;
    }

    #noBtn {
      background-color: #999;
      color: white;
      position: absolute;
    }

    .heart {
      position: absolute;
      color: #ff3366;
      font-size: 22px;
      animation: float 5s linear infinite;
    }

    @keyframes float {
      from {
        transform: translateY(100vh);
        opacity: 1;
      }
      to {
        transform: translateY(-10vh);
        opacity: 0;
      }
    }
  </style>
</head>

<body>

  <!-- 🎵 Background Music -->
  <audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-love.mp3" type="audio/mpeg">
  </audio>

  <div class="container" id="main">
    <h1>💖 Januu 💖</h1>
    <h2>Will you be my Valentine? 💘</h2>

    <button id="yesBtn" onclick="yesClicked()">Yes 💕</button>
    <button id="noBtn" onmouseover="moveNo()">No 💔</button>
  </div>

  <script>
    const noBtn = document.getElementById("noBtn");

    function moveNo() {
      const x = Math.random() * (window.innerWidth - 120);
      const y = Math.random() * (window.innerHeight - 60);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    }

    function yesClicked() {
      document.body.innerHTML = `
        <div class="container">
          <h1>💖 Happy Valentine’s Day 💖</h1>
          <p style="font-size:22px; color:#ff3366;">
            You just made my heart skip a beat 💕<br><br>
            Every smile of yours is my favorite place ✨<br><br>
            Thank you for being my Valentine 💘
          </p>
          <p style="font-size:18px;">Forever yours 💌</p>
        </div>
      `;
    }

    // Floating hearts
    setInterval(() => {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerHTML = "❤";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (3 + Math.random() * 3) + "s";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 5000);
    }, 300);
  </script>

</body>
</html>
