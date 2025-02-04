<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pedirle ser mi San Valentín</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1 id="titulo">HOLA FLAQUI, ¿QUIERES SER MI CITA PARA EL 14 DE FEBRERO? DI QUE SI PORFA</h1>
        <div class="botones">
            <button id="no" class="boton">NO</button>
            <button id="si" class="boton">SI</button>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background-color: #FADCD9; /* Color rosado bebé */
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    overflow: hidden;
}

.container {
    text-align: center;
}

h1 {
    font-size: 2.5rem;
    color: #D86A6A;
    animation: moverTitulo 2s ease-in-out;
}

@keyframes moverTitulo {
    0% { transform: translateX(-100%); }
    50% { transform: translateX(0); }
    100% { transform: translateX(100%); }
}

.botones {
    margin-top: 20px;
}

.boton {
    background-color: #D86A6A;
    color: white;
    border: none;
    padding: 10px 20px;
    font-size: 1.2rem;
    cursor: pointer;
    transition: transform 0.3s, background-color 0.3s;
}

.boton:hover {
    transform: scale(1.1);
    background-color: #F5A9A9;
}

#no {
    position: relative;
}

#no.mover {
    position: absolute;
    left: 100vw;
    transition: left 0.5s ease-out;
}

const botonNo = document.getElementById('no');
const botonSi = document
