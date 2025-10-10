<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RL Software - Benvenuto</title>
    <style>
        /* Stili di base */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 20px;
        }

        h1 {
            font-size: 3rem;
            letter-spacing: 1px;
        }

        /* Navbar */
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            margin-top: 15px;
        }

        nav ul li {
            margin: 0 25px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
        }

        nav ul li a:hover {
            color: #1abc9c;
        }

        /* Sezione Contatti */
        #contact {
            padding: 60px 0;
            background-color: #ecf0f1;
            text-align: center;
        }

        #contact h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        #contact p {
            font-size: 1.2rem;
            margin-bottom: 40px;
        }

        .email-container {
            position: relative;
            display: inline-block;
        }

        .copy-button {
            background-color: #1abc9c;
            color: white;
            font-size: 1.1rem;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            border: none;
            transition: background-color 0.3s ease;
        }

        .copy-button:hover {
            background-color: #16a085;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #2c3e50;
            color: white;
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>RL Software - Home</h1>
        <nav>
            <ul>
                <li><a href="README.md">Home</a></li>
                <li><a href="games.md">Videogiochi</a></li>
                <li><a href="#contact">Contattaci</a></li>
            </ul>
        </nav>
    </header>

    <!-- Sezione di Contatti -->
    <section id="contact">
        <h2>Contattaci</h2>
        <p>Se hai bisogno di supporto, hai domande o vuoi caricare anche tu un gioco, puoi contattarci via email:</p>
        
        <!-- Sezione della mail con il pulsante per copiare -->
        <div class="email-container">
            <strong>Email: <span id="email">software.rl25@gmail.com</span></strong>
            <button class="copy-button" onclick="copyEmail()">Copia Email</button>
        </div>
        
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 RL Software. Tutti i diritti riservati.</p>
    </footer>

    <script>
        // Funzione per copiare la mail negli appunti
        function copyEmail() {
            const email = document.getElementById('email').textContent;
            const textArea = document.createElement('textarea');
            textArea.value = email;
            document.body.appendChild(textArea);
            textArea.select();
            document.execCommand('copy');
            document.body.removeChild(textArea);
            
            // Mostra un messaggio che indica che la mail è stata copiata
            alert("Email copiata negli appunti: " + email);
        }
    </script>

</body>
</html>
