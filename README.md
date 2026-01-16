# Telegram-Gaming-Mini-App<!DOCTYPE html>
<html>
<head>
  <title>Telegram Game</title>
  <script src="https://telegram.org/js/telegram-web-app.js"></script>
</head>
<body>
  <h2>🎮 Welcome to My Telegram Game</h2>

  <button onclick="playGame()">Play Game</button>
  <p id="result"></p>

  <script>
    const tg = window.Telegram.WebApp;
    tg.expand();

    function playGame() {
      let dice = Math.floor(Math.random() * 6) + 1;
      document.getElementById("result").innerText =
        "🎲 Dice Result: " + dice;
    }
  </script>
</body>
</html>
