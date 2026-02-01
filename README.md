# index.html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<h1>Will you be my Valentine, <span class="name">Beba</span>? 💖</h1>
  
<style>
  body {
    margin: 0;
    height: 100vh;
    background: linear-gradient(135deg, #ff758c, #ff7eb3);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Poppins', sans-serif;
    color: white;
    text-align: center;
  }

  .card {
    background: rgba(255,255,255,0.15);
    padding: 40px;
    border-radius: 20px;
    backdrop-filter: blur(10px);
  }

  h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
  }

  p {
    font-size: 1.2rem;
    margin-bottom: 30px;
  }

  button {
    padding: 12px 25px;
    font-size: 1.1rem;
    border: none;
    border-radius: 30px;
    cursor: pointer;
    margin: 10px;
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

.name {
  color: #fff;
  font-weight: 600;
}

</style>
</head>
<body>

<div class="card">
  <h1>Will you be my Valentine? 💖</h1>
  <p>You make my every day better. So… what do you say? 🌹</p>
  <button id="yes" onclick="yesClicked()">YES 💕</button>
  <button id="no">NO 🙄</button>
</div>

<script>
  const noBtn = document.getElementById("no");

  noBtn.addEventListener("mouseover", () => {
    const x = Math.random() * (window.innerWidth - 100);
    const y = Math.random() * (window.innerHeight - 50);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
  });

  function yesClicked() {
    document.body.innerHTML = `
      <div style="text-align:center; color:white;">
        <h1>YAYYYY 💘</h1>
        <p style="font-size:1.5rem;">
          Best decision ever 🥰<br>
          I can’t wait to celebrate love with you ❤️
        </p>
      </div>
    `;
  }
</script>

</body>
</html>
