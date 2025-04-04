<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Alice e Michel</title>
  <style>
    body {
      margin: 0;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      background: linear-gradient(to bottom, #fceabb, #f8b500);
      animation: backgroundChange 10s infinite alternate;
    }

    @keyframes backgroundChange {
      0% { background-color: #fceabb; }
      100% { background-color: #ffb347; }
    }

    header {
      padding: 20px;
      background: #fff;
      color: #000;
      font-size: 2em;
      text-align: center;
      font-weight: bold;
    }

    #clock {
      position: absolute;
      top: 10px;
      right: 20px;
      font-size: 1em;
      color: #000;
    }

    nav {
      background-color: #fff;
      padding: 10px;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 10px;
    }

    nav a {
      text-decoration: none;
      color: #000;
      background: #ffe680;
      padding: 10px 20px;
      border-radius: 10px;
      font-weight: bold;
    }

    section {
      padding: 20px;
    }

    .love-message {
      text-align: center;
      font-size: 1.2em;
      color: #fff;
      animation: loveFade 6s infinite;
    }

    @keyframes loveFade {
      0% { opacity: 0; }
      50% { opacity: 1; }
      100% { opacity: 0; }
    }
  </style>
</head>
<body>
  <div id="clock"></div>
  <header>Alice e Michel</header>
  <div class="love-message">Ti amo ogni giorno di più</div>
  <nav>
    <a href="#">Entrate / Uscite</a>
    <a href="#">Spese mensili fisse</a>
    <a href="#">Michel lavoro</a>
    <a href="#">Alice lavoro</a>
    <a href="#">Documenti</a>
    <a href="#">Percorso Michel</a>
    <a href="#">Cassetto dei desideri</a>
    <a href="#">Agenda - Calendario</a>
  </nav>

  <section>
    <p>Benvenuti nel nostro spazio personale!</p>
    <p>Qui potete gestire le vostre spese, documenti, e molto altro.</p>
  </section>

  <script>
    function updateClock() {
      const now = new Date();
      const clock = document.getElementById('clock');
      clock.textContent = now.toLocaleString();
    }
    setInterval(updateClock, 1000);
    updateClock();
  </script>
</body>
</html>