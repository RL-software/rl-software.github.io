<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>RL Software</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f5f5f5;
      color: #222;
    }
    header {
      background: #000;
      color: #fff;
      padding: 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    header .logo {
      font-size: 24px;
      font-weight: bold;
    }
    nav a {
      color: #fff;
      margin: 0 15px;
      text-decoration: none;
    }
    .hero {
      background: #fff;
      text-align: center;
      padding: 100px 20px;
    }
    .hero h1 {
      margin: 0 0 20px;
      font-size: 48px;
      color: #000;
    }
    .hero button {
      padding: 15px 30px;
      font-size: 18px;
      background: #000;
      color: #fff;
      border: none;
      cursor: pointer;
    }
    .games {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
      padding: 40px;
    }
    .game-card {
      background: #fff;
      border: 1px solid #ddd;
      border-radius: 8px;
      overflow: hidden;
      display: flex;
      flex-direction: column;
    }
    .game-card img {
      width: 100%;
      height: auto;
    }
    .game-card .info {
      padding: 15px;
      flex: 1;
    }
    .game-card .info h3 {
      margin: 0 0 10px;
    }
    .game-card .info button {
      margin-top: auto;
      padding: 10px;
      background: #000;
      color: #fff;
      border: none;
      cursor: pointer;
      width: 100%;
    }
    footer {
      background: #000;
      color: #fff;
      padding: 20px;
      text-align: center;
    }
    .contact-form {
      max-width: 500px;
      margin: 0 auto;
    }
    .contact-form input, .contact-form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    .contact-form button {
      background: #000;
      color: #fff;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">RL Software</div>
    <nav>
      <a href="#">Home</a>
      <a href="#games">Giochi</a>
      <a href="#download">Scarica</a>
      <a href="#contacts">Contatti</a>
      <a href="#account">Account</a>
    </nav>
  </header>

  <section class="hero" id="home">
    <h1>Benvenuto su RL Software</h1>
    <button onclick="scrollToSection('games')">Scarica Ora</button>
  </section>

  <section class="games" id="games">
    <div class="game-card">
      <img src="placeholder.jpg" alt="Gioco 1">
      <div class="info">
        <h3>Gioco 1</h3>
        <p>Descrizione breve...</p>
        <button>Download</button>
      </div>
    </div>
    <div class="game-card">
      <img src="placeholder2.jpg" alt="Gioco 2">
      <div class="info">
        <h3>Gioco 2</h3>
        <p>Descrizione breve...</p>
        <button>Download</button>
      </div>
    </div>
    <!-- altri giochi -->
  </section>

  <section id="contacts">
    <h2>Contattaci</h2>
    <div class="contact-form">
      <form action="mailto:software.rl25@gmail.com" method="post" enctype="text/plain">
        <input type="text" name="name" placeholder="Nome" required>
        <input type="email" name="email" placeholder="Email" required>
        <textarea name="message" rows="5" placeholder="Messaggio" required></textarea>
        <button type="submit">Invia Messaggio</button>
      </form>
      <p>Oppure scrivici direttamente a: <strong>software.rl25@gmail.com</strong></p>
    </div>
  </section>

  <footer>
    &copy; 2025 RL Software. Tutti i diritti riservati.
  </footer>

  <script>
    function scrollToSection(id) {
      const el = document.getElementById(id);
      if (el) {
        el.scrollIntoView({ behavior: "smooth" });
      }
    }
  </script>

</body>
</html>
