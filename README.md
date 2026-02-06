<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Ma Valentine 💘</title>
<style>
  body {
    background: #ffe6f0;
    font-family: Arial, sans-serif;
    text-align: center;
    margin-top: 100px;
  }

  h1 {
    color: #ff2e63;
  }

  .btn {
    padding: 15px 25px;
    font-size: 18px;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    margin: 20px;
    position: relative;
  }

  #yesBtn {
    background-color: #ff2e63;
    color: white;
  }

  #noBtn {
    background-color: #999;
    color: white;
    position: absolute;
  }
</style>
</head>

<body>

<h1>Veux-tu être ma Valentine ? 💕</h1>

<button id="yesBtn" class="btn" onclick="yes()">Oui 💖</button>
<button id="noBtn" class="btn">Non 😈</button>

<script>
function yes() {
  document.body.innerHTML = "<h1>YEEEEES 💘🥰</h1><p>je t'aime mon bb</p>";
}

const noBtn = document.getElementById("noBtn");

noBtn.addEventListener("mouseover", moveButton);
noBtn.addEventListener("click", moveButton);

function moveButton() {
  const x = Math.random() * (window.innerWidth - 100);
  const y = Math.random() * (window.innerHeight - 50);
  noBtn.style.left = x + "px";
  noBtn.style.top = y + "px";
}
</script>

</body>
</html>
