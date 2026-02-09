# Login-simulado
projeto-6-login
<!DOCTYPE html>
<html>
<head>
  <title>Login</title>
</head>
<body>

<input id="user" placeholder="Usuário">
<input id="pass" type="password" placeholder="Senha">
<button onclick="login()">Entrar</button>

<p id="msg"></p>

<script src="script.js"></script>
</body>
</html>
function login() {
  const user = document.getElementById("user").value;
  const pass = document.getElementById("pass").value;

  if (user === "admin" && pass === "123") {
    document.getElementById("msg").textContent = "Login realizado!";
  } else {
    document.getElementById("msg").textContent = "Dados inválidos";
  }
}
