<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Will You Be My Valentine?</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Poppins', sans-serif;
      color: white;
      text-align: center;
      padding: 20px;
    }

    .card {
      width: 100%;
      max-width: 380px;
      background: rgba(255, 255, 255, 0.18);
      padding: 30px 20px;
      border-radius: 22px;
      backdrop-filter: blur(10px);
    }

    h1 {
      font-size: 1.8rem;
      margin-bottom: 12px;
    }

    .name {
      font-weight: 600;
    }

    p {
      font-size: 1rem;
      margin-bottom: 20px;
      line-height: 1.4;
    }

    .photos {
      display: flex;
      gap: 12px;
      overflow-x: auto;
      padding-bottom: 10px;
      margin-bottom: 25px;
    }

    .photos img {
      height: 160px;
      border-radius: 16px;
      flex-shrink: 0;
    }

    .buttons {
      display: flex;
      flex-direction: column;
      gap: 15px;
      align-items: center;
    }

    button {
      width: 100%;
      max-width: 220px;
      padding: 14px;
      font-size: 1rem;
      border: none;
      border-radius: 999px;
      cursor: pointer;
    }

    #yes {
      background: #ff4d6d;
      color: white;
    }

    #no {
      background: white;
      color: #ff4d6d;
      position: absolute;
    }
  </style>
</head>

<body>

  <div class="card">
    <h1>Will you be my Valentine, <span class="name">Beba</span>? 💖</h1>

    <p>You make my every day better. So… what do you say? 🌹</p>

  <div class="photos">
  <img src="pic1.jpg" alt="Us">
  <img src="pic2.jpg" alt="Us">
  <img src="pic3.jpg" alt="Us">
  <img src="pic4.jpg" alt="Us">
  <img src="pic5.jpg" alt="Us">
  <img src="pic6.jpg" alt="Us">
</div>

  </div>

  <script>
    const noBtn = document.getElementById("no");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 120);
      const y = Math.random() * (window.innerHeight - 60);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });

    function yesClicked() {
      document.body.innerHTML = `
        <div style="text-align:center; color:white;">
          <h1>YAYYYY 💘</h1>
          <p style="font-size:1.4rem;">
            Officially my Valentine 💕<br>
            I love you endlessly ❤️
          </p>
        </div>
      `;
    }
  </script>

</body>
</html>
