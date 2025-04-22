# amoolucas
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Surpresa!</title>
  <style>
    body {
      background-color: #fceaff;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      flex-direction: column;
      font-family: 'Comic Sans MS', cursive;
    }

    button {
      padding: 15px 30px;
      font-size: 20px;
      background-color: #ff66c4;
      border: none;
      border-radius: 20px;
      color: white;
      cursor: pointer;
      box-shadow: 0 0 20px #ff66c4;
      transition: 0.3s;
    }

    button:hover {
      background-color: #ff33aa;
      box-shadow: 0 0 25px #ff33aa;
    }

    .mensagem {
      margin-top: 40px;
      font-size: 30px;
      font-weight: bold;
      color: #ff66c4;
      display: none;
      animation: brilhar 1s infinite alternate, mexer 2s infinite ease-in-out;
    }

    @keyframes brilhar {
      0% { text-shadow: 0 0 5px #ff66c4, 0 0 10px #ff99cc; }
      100% { text-shadow: 0 0 20px #ff66c4, 0 0 30px #ff99cc; }
    }

    @keyframes mexer {
      0% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0); }
    }
  </style>
</head>
<body>

  <button onclick="mostrarMensagem()">Clica aqui!</button>

  <div class="mensagem" id="mensagem">
    Eu te amo, Lucas! Tu é meu solzinho!
  </div>

  <script>
    function mostrarMensagem() {
      document.getElementById('mensagem').style.display = 'block';
    }
  </script>

</body>
</html>