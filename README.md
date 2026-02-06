<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Pour toi ❤️</title>

<style>
body {
  margin: 0;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(135deg, #ff9a9e, #fad0c4);
  font-family: Arial, sans-serif;
}

.container {
  text-align: center;
  background: white;
  padding: 40px;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.2);
}

h1 {
  font-size: 32px;
  color: #ff4d6d;
}

button {
  padding: 15px 25px;
  font-size: 18px;
  margin: 10px;
  border: none;
  border-radius: 10px;
  cursor: pointer;
  transition: 0.3s;
}

#yes {
  background-color: #ff4d6d;
  color: white;
}

#no {
  background-color: #ccc;
}
</style>
</head>

<body>

<div class="container">
  <h1>Veux-tu être ma Valentine ? 💌</h1>
  <button id="yes" onclick="yes()">Oui ❤️</button>
  <button id="no" onmouseover="moveNo()">Non 😏</button>
</div>

<script>
function yes() {
  document.querySelector(".container").innerHTML =
    "<h1>YEEEEES ❤️🥰</h1><p>je t'aime mon ange rendez vous le 13 j'aurais une petite surprise pour toi</p>";
}

function moveNo() {
  const btn = document.getElementById("no");
  btn.style.position = "absolute";
  btn.style.top = Math.random() * 80 + "%";
  btn.style.left = Math.random() * 80 + "%";
}
</script>

</body>
</html>
