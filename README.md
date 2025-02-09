<Espero que te guste mucho mi amor❤️>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(to bottom, #f8cdda, #1d2b64);
            color: #fff;
            text-align: center;
            padding: 0;
            margin: 0;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            box-sizing: border-box;
        }

        h1 {
            font-size: 3.8em;
            font-family: 'Dancing Script', cursive;
            color: #ffb3b3;
            margin-bottom: 20px;
        }

        p {
            font-size: 1.5em;
            margin-bottom: 30px;
            color: #f1f1f1;
            line-height: 1.5;
        }

        .heart {
            font-size: 6em;
            color: #ff4d94;
            margin-bottom: 30px;
            animation: heartbeat 1.5s infinite;
        }

        /* Button Styles */
        .button {
            background: linear-gradient(45deg, #ff66b2, #ff1e6c);
            color: white;
            font-size: 1.5em;
            padding: 20px 40px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease-in-out;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            margin: 10px;
            width: 200px;
        }

        .button:hover {
            transform: scale(1.1);
            background: linear-gradient(45deg, #ff1e6c, #ff66b2);
        }

        .button:focus {
            outline: none;
        }

        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }

        .footer {
            margin-top: 40px;
            font-size: 1.2em;
            color: #ffb3b3;
        }

        /* Thank you message */
        .thank-you-message, .no-thank-you-message {
            font-size: 2.2em;
            color: #ff66b2;
            font-family: 'Dancing Script', cursive;
            opacity: 0;
            visibility: hidden; /* Añadido para ocultar los mensajes inicialmente */
            transition: opacity 1s ease-in-out;
            margin-top: 20px;
            text-align: center;
        }

        /* Soft shadow for elegance */
        h1, p, .button {
            text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.3);
        }

        /* Custom message styles */
        .no-thank-you-message {
            color: #ff4d94;
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Reproductor de música -->
    <audio id="music" autoplay loop>
        <source src="tu_musica.mp3" type="audio/mp3">
        Tu navegador no soporta el elemento de audio.
    </audio>

    <h1 id="question">¿Quieres ser mi San Valentín?</h1>
    <p>Desde el primer día que te conocí, mi vida cambió. Este San Valentín quiero compartirlo contigo. 💖</p>
    <div class="heart">❤️</div>
    <!-- Botones de sí y no -->
    <div id="buttons">
        <button class="button" onclick="showThankYouMessage()">¡Sí, claro! 💕</button>
        <button class="button" onclick="showNoThanksMessage()">No, gracias 😞</button>
    </div>
    <div class="footer">
        *Haz clic para responder 😉
    </div>

    <!-- Mensaje de agradecimiento que aparecerá después -->
    <div id="thankYouMessage" class="thank-you-message">
        ¡Muchas gracias por aceptar mi amor! Te amo mushooooooooooo 💖
    </div>

    <!-- Mensaje de respuesta negativa -->
    <div id="noThanksMessage" class="no-thank-you-message">
        ¡Oh no! 😭 Te seguiré queriendo de todos modos. 💔
    </div>

    <script>
        // Mostrar el mensaje de agradecimiento
        function showThankYouMessage() {
            // Ocultar la pregunta y los botones
            document.getElementById('question').style.display = 'none';
            document.getElementById('buttons').style.display = 'none';

            // Mostrar el mensaje de agradecimiento con transición
            const thankYouMessage = document.getElementById('thankYouMessage');
            thankYouMessage.style.visibility = 'visible';
            thankYouMessage.style.opacity = 1;
        }

        // Mostrar el mensaje de rechazo
        function showNoThanksMessage() {
            // Ocultar la pregunta y los botones
            document.getElementById('question').style.display = 'none';
            document.getElementById('buttons').style.display = 'none';

            // Mostrar el mensaje de rechazo con transición
            const noThanksMessage = document.getElementById('noThanksMessage');
            noThanksMessage.style.visibility = 'visible';
            noThanksMessage.style.opacity = 1;
        }
    </script>
</body>
</html>
