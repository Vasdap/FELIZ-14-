<BUENAS>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Jhoana 💖</title>
    <style>
        body {
            text-align: center;
            background: pink;
            background-image: url('https://img.freepik.com/vector-premium/patron-costuras-lindo-capibara-animal-sobre-fondo-rosa_248911-2592.jpg?w=740');
            background-size: video;
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
        <h1>Hola amor, ¿quieres ser mi San Valentín? 💘</h1>
        <div class="buttons">
            <button class="btn yes" onclick="aceptar()">¡Sí! 💖</button>
            <button class="btn no" onmouseover="moverBoton()">No 😢</button>
        </div>
    </div>
    
   <script>
        function aceptar() {
         var mensaje = document.createElement("div");
        mensaje.innerHTML = "¡Sabía que dirías que sí! 💕🥰 TE AMOOOOOO, nos vemos pronto en el retiro";
        
        
        mensaje.style.fontSize = "20px";
        mensaje.style.fontWeight = "bold";
        mensaje.style.color = "black";
        mensaje.style.textAlign = "center";
        mensaje.style.marginTop = "20px";
        mensaje.style.opacity = "1"; 
        mensaje.style.transition = "all 1s ease"; 
        
    
        document.body.appendChild(mensaje);

      
        setTimeout(function() {
            mensaje.style.opacity = "1";
            mensaje.style.fontSize = "30px"; // Aumentar el tamaño del texto para que "crezca"
        }, 100);

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
