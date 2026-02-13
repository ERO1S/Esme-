<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sincronicidad</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            background-color: #0d0d0d; /* Negro profundo */
            color: #f2f2f2;
            font-family: 'Georgia', serif;
            overflow: hidden;
        }

        .container {
            text-align: center;
            max-width: 600px;
            padding: 20px;
            z-index: 2;
        }

        /* Contenedor del Corazón SVG */
        .heart-svg {
            width: 150px;
            height: 150px;
            filter: drop-shadow(0 0 15px rgba(179, 57, 57, 0.8));
            animation: heartbeat 1.5s ease-in-out infinite;
            cursor: pointer;
        }

        path {
            fill: #b33939; /* Rojo elegante */
        }

        /* Animación de latido realista */
        @keyframes heartbeat {
            0% { transform: scale(1); }
            15% { transform: scale(1.15); }
            30% { transform: scale(1); }
            45% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        .line {
            height: 1px;
            width: 80px;
            background: linear-gradient(to right, transparent, #b33939, transparent);
            margin: 30px auto;
        }

        h1 {
            font-weight: lighter;
            letter-spacing: 4px;
            color: #e67e22; /* Color cálido */
            text-transform: uppercase;
            font-size: 1.2rem;
        }

        p {
            line-height: 1.8;
            font-size: 1.1rem;
            font-style: italic;
            color: #cccccc;
        }

        /* Pequeñas partículas de fondo (Opcional) */
        .bg-dots {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background-image: radial-gradient(#333 1px, transparent 1px);
            background-size: 30px 30px;
            opacity: 0.3;
            z-index: 1;
        }
    </style>
</head>
<body>

    <div class="bg-dots"></div>

    <svg class="heart-svg" viewBox="0 0 32 32">
        <path d="M16 28.5c-.5 0-1-.2-1.4-.5l-10.4-9.3C2.1 16.8 1 14.7 1 12.3 1 7.7 4.7 4 9.3 4c2.2 0 4.3.9 5.8 2.4l.9.9.9-.9c1.5-1.5 3.6-2.4 5.8-2.4 4.6 0 8.3 3.7 8.3 8.3 0 2.4-1.1 4.5-3.2 6.4l-10.4 9.3c-.4.3-.9.5-1.4.5z"/>
    </svg>

    <div class="container">
        <h1>TQM</h1>
        <div class="line"></div>
        <p>
            Si fueras un error de compilación en mi código, probablemente dejaría de buscar la solución solo para que te quedaras ahí un rato más
        </p>
    </div>

</body>
</html>

