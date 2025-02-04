<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Jhoana ❤️</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: pink;
            overflow: hidden;
            color: black;
        }
        h1 {
            color: black;
            margin-top: 50px;
            animation: heartbeat 1.5s infinite ease-in-out;
        }
        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
        .sticker {
            width: 150px;
            margin-top: 20px;
        }
        .btn-container {
            margin-top: 20px;
            position: relative;
        }
        .btn {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 10px;
        }
        .yes {
            background-color: lightgreen;
        }
        .no {
            background-color: lightcoral;
            position: absolute;
            transition: transform 0.2s ease-in-out;
        }
        .heart {
            position: absolute;
            color: red;
            font-size: 20px;
            animation: float 5s infinite ease-in-out;
        }
        @keyframes float {
            0% { transform: translateY(0); opacity: 1; }
            100% { transform: translateY(-600px); opacity: 0; }
        }
    </style>
</head>
<body>
    <h1>Jhoana, ¿quieres ser mi San Valentín? ❤️</h1>
    <img src="sticker.png" alt="Sticker lindo" class="sticker">
    <div class="btn-container">
        <button class="btn yes" onclick="accept()">Sí 😍</button>
        <button class="btn no" onmousemove="moveNoButton()">No 😢</button>
    </div>
    <audio autoplay loop>
        <source src="tu-cancion-romantica.mp3" type="audio/mpeg">
        Tu navegador no soporta audio.
    </audio>
    <script>
        function moveNoButton() {
            const noBtn = document.querySelector('.no');
            const x = Math.random() * (window.innerWidth - 100);
            const y = Math.random() * (window.innerHeight - 50);
            noBtn.style.transform = `translate(${x}px, ${y}px)`;
        }
        function accept() {
            alert('¡Sabía que dirías que sí! ❤️ Te amo 😘');
        }
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * window.innerWidth + 'px';
            heart.style.top = window.innerHeight + 'px';
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 5000);
        }
        setInterval(createHeart, 500);
    </script>
</body>
</html>

            setTimeout(() => heart.remove(), 5000);
        }
        setInterval(createHeart, 500);
    </script>
</body>
</html>
