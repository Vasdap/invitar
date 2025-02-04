<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>San Valentín para Jhoana</title>
    <style>
        body {
            background-color: #f8c8dc;
            text-align: center;
            font-family: Arial, sans-serif;
            animation: fadeIn 2s ease-in-out;
            position: relative;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        h1 {
            color: #d63384;
            font-size: 2em;
            margin-top: 20vh;
            animation: bounce 1.5s infinite;
        }
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        .buttons {
            margin-top: 40px;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            position: relative;
        }
        .btn {
            font-size: 1.5em;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
            transition: transform 0.3s;
        }
        .btn:hover {
            transform: scale(1.1);
        }
        .yes {
            background-color: #ff69b4;
            color: white;
        }
        .no {
            background-color: #ffcccb;
            color: black;
            position: relative;
        }
        .heart {
            position: absolute;
            top: 10%;
            left: 50%;
            transform: translateX(-50%);
            font-size: 5em;
            color: red;
            animation: heartbeat 1s infinite;
        }
        @keyframes heartbeat {
            0%, 100% { transform: translateX(-50%) scale(1); }
            50% { transform: translateX(-50%) scale(1.2); }
        }
    </style>
</head>
<body>
    <div class="heart">❤️</div>
    <h1>HOLA FLAQUI, ¿QUIERES SER MI CITA PARA EL 14 DE FEBRERO? DI QUE SI PORFA</h1>
    <div class="buttons">
        <button class="btn yes" onclick="alert('¡Sabía que dirías que sí! 💖')">Sí</button>
        <button class="btn no" id="noBtn">No</button>
    </div>
    
    <script>
        document.getElementById("noBtn").addEventListener("mouseover", function() {
            let x = Math.random() * (window.innerWidth - this.offsetWidth);
            let y = Math.random() * (window.innerHeight - this.offsetHeight);
            this.style.left = `${x}px`;
            this.style.top = `${y}px`;
        });
    </script>
</body>
</html>
