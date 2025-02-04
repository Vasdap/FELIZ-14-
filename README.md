<!DOCTYPE html>
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
            background-image: url('2a8cd4e2029644a3d8cdcfa279e97c60.jpg'); /* Fondo de capibara */
            background-size: cover;
            background-position: center;
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
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 10px;
            margin-top: 20px;
            padding: 10px;
        }
        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 10px;
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
        <div class="gallery">
            <img src="WhatsApp Image 2025-02-03 at 8.07.19 PM (2).jpeg" alt="Foto 1![WhatsApp Image 2025-02-03 at 8 07 18 PM (2)](https://github.com/user-attachments/assets/ae302649-b137-4eb9-b633-1fb84df91e66)
" >
            <img src="WhatsApp Image 2025-02-03 at 8.07.17 PM (2).jpeg" alt="Foto 2"![WhatsApp Image 2025-02-03 at 8 07 19 PM](https://github.com/user-attachments/assets/5dca7474-d665-43cf-82af-d6c74573724c)
 >
            <img src="imagen3.jpg" alt="Foto 3"![WhatsApp Image 2025-02-03 at 8 07 17 PM (2)](https://github.com/user-attachments/assets/6b8d3975-6c52-4ff0-88e0-e7ebcc4d6646)>

            <img src="imagen4.jpg" alt="Foto 4"![WhatsApp Image 2025-02-03 at 8 07 19 PM (1)](https://github.com/user-attachments/assets/f71e2dc2-07a8-4065-ba4f-57e9aa9e6790)
 >
        </div>
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
