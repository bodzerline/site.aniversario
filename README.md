# site.aniversario<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Feliz Aniversário, Amor!</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #ffe4ec;
      color: #5c1a33;
      margin: 0;
      padding: 0;
      text-align: center;
    }
    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
    }
    .hidden { display: none; }
    input[type="password"] {
      padding: 10px;
      margin-top: 20px;
      font-size: 16px;
    }
    button {
      padding: 10px 20px;
      margin-top: 10px;
      background-color: #ff69b4;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }
    button:hover {
      background-color: #ff1493;
    }
    .quiz-question {
      margin: 20px 0;
    }
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-romantic.mp3" type="audio/mp3">
  </audio>
  
  <div class="container">
    <div id="login">
      <h2>Digite a senha para acessar 💌</h2>
      <input type="password" id="senha" placeholder="Senha">
      <button onclick="verificarSenha()">Entrar</button>
    </div>

    <div id="conteudo" class="hidden">
      <h1>Feliz Aniversário, meu Amor! 🎉</h1>
      <p>Hoje é um dia especial porque é o seu dia. Eu sou tão grata por ter você na minha vida. Espero que esse site te faça sorrir tanto quanto você me faz sorrir todos os dias 💖</p>

      <h2>Nosso Quiz 💕</h2>
      <div class="quiz-question">
        <p><strong>1. Onde foi nosso primeiro encontro?</strong></p>
        <button>Parque</button>
        <button>Cinema</button>
        <button>Restaurante</button>
      </div>

      <div class="quiz-question">
        <p><strong>2. Qual é sua cor favorita?</strong></p>
        <button>Azul</button>
        <button>Preto</button>
        <button>Rosa</button>
      </div>

      <div class="quiz-question">
        <p><strong>3. Qual música é a nossa?</strong></p>
        <button>Perfect - Ed Sheeran</button>
        <button>Thinking Out Loud</button>
        <button>Nosso cover no karaokê 🎤</button>
      </div>

      <p style="margin-top: 30px;">Te amo infinitamente! 💘</p>
    </div>
  </div>

  <script>
    function verificarSenha() {
      const senha = document.getElementById('senha').value;
      const senhaCorreta = '1234'; // Altere aqui sua senha personalizada

      if (senha === senhaCorreta) {
        document.getElementById('login').classList.add('hidden');
        document.getElementById('conteudo').classList.remove('hidden');
      } else {
        alert('Senha incorreta!');
      }
    }
  </script>
</body>
</html>
