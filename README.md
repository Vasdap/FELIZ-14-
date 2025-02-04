<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jhoana, ¿quieres ser mi San Valentín?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffcccb;
        }
        .container {
            margin-top: 100px;
        }
        .buttons {
            margin-top: 20px;
            position: relative;
        }
        .btn {
            font-size: 20px;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
        }
        .yes {
            background-color: #4CAF50;
            color: white;
        }
        .no {
            background-color: #f44336;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Jhoana, ¿quieres ser mi San Valentín? 💘</h1>
        <div class="buttons">
            <button class="btn yes" onclick="aceptar()">Sí</button>
            <button class="btn no" id="botonNo">No</button>
        </div>
        <p id="mensaje" style="font-size: 24px; font-weight: bold; margin-top: 20px;"></p>
    </div>

    <script>
        function moverBoton() {
            let botonNo = document.getElementById("botonNo");
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            botonNo.style.left = `${x}px`;
            botonNo.style.top = `${y}px`;
        }

        function aceptar() {
            document.getElementById("mensaje").innerText = "¡Sabía que dirías que sí!\nTE AMO FLAQUI ❤️";
        }

        document.getElementById("botonNo").addEventListener("mouseover", moverBoton);
    </script>
</body>
</html>

