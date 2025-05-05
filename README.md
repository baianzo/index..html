<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ваш аккаунт взломан</title>
  <style>
    body {
      margin: 0;
      background-color: black;
      color: lime;
      font-family: monospace;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
    }
    #message {
      text-align: center;
      font-size: 1.5rem;
      white-space: pre-line;
    }
    .hidden {
      display: none;
    }
    .blink {
      animation: blink 1s step-start infinite;
    }
    @keyframes blink {
      50% { opacity: 0; }
    }
  </style>
</head>
<body>
  <div id="message">
    <span class="blink">Ваш аккаунт был взломан...</span>
    <br><br>
    Загружаем данные...
  </div>

  <script>
    setTimeout(() => {
      document.body.style.backgroundColor = '#fff';
      document.body.style.color = '#000';
      document.getElementById('message').innerHTML = `🎉 ЭТО ШУТКА!\\n\\nТы не взломан.\\nНо всё равно — будь осторожен в интернете! 😄`;
    }, 5000);
  </script>
</body>
</html>
