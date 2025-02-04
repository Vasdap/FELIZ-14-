<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Jhoana 💖</title>
    <style>
        body {
            text-align: above;
            background: pink;
            background-image: url('https://media.istockphoto.com/id/2153094727/es/vector/couple-of-capybaras-in-love.jpg?s=612x612&w=0&k=20&c=LFLcTkAwwHOy2eTH49b3n9C9F5pWTrNngETgBJ3VPAc=');
            background-size: cover;
            font-family: Arial, sans-serif;
        }
        .container {
            margin-top: 100px;
            background: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
            display: inline-block;
        }
        h1 {
            color: #ff3366;
            font-size: 3rem;
        }
        .buttons {
            margin-top: 20px;
        }
        .btn {
            font-size: 1.5rem;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }
        .yes {
            background-color: #ff3366;
            color: white;
        }
        .yes:hover {
            background-color: #ff6699;
        }
        .no {
            background-color: #666;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Jhoana, ¿quieres ser mi San Valentín? 💘</h1>
        <div class="buttons">
            <button class="btn yes" onclick="aceptar()">¡Sí! 💖</button>
            <button class="btn no" onmouseover="moverBoton()">No 😢</button>
        </div>
    </div>
    
    <script>
        function aceptar() {
            alert("¡Sabía que dirías que sí! 💕🥰");
        }
        
        function moverBoton() {
            let noButton = document.querySelector('.no');
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            noButton.style.left = `${x}px`;
            noButton.style.top = `${y}px`;
        }
    </script>
</body>
</html>
