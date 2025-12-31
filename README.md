<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aprendizaje con IA</title>

    <style>
        /* ================= CONFIGURACIÓN GENERAL ================= */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, sans-serif;
        }

        body {
            background-color: #05010d;
            color: #ffffff;
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* ================= HEADER ================= */
        .header {
            position: relative;
            min-height: 100vh;
            background: radial-gradient(circle at top, #12002b, #05010d 70%);
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            overflow: hidden;
        }

        .header-content {
            position: relative;
            z-index: 2;
            max-width: 800px;
            padding: 2rem;
        }

        .header-content h1 {
            font-size: 2.8rem;
            margin-bottom: 1rem;
            text-shadow: 0 0 15px #7f00ff;
        }

        .header-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            color: #cfc9ff;
        }

        /* ================= BOTÓN NEÓN ================= */
        .btn-neon {
            display: inline-block;
            padding: 0.8rem 2rem;
            color: #00ffff;
            border: 2px solid #00ffff;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            box-shadow: 0 0 10px #00ffff;
            transition: all 0.3s ease;
        }

        .btn-neon:hover {
            background: #00ffff;
            color: #05010d;
            box-shadow: 0 0 25px #00ffff;
        }

        /* ================= SECCIÓN ================= */
        .section {
            padding: 4rem 2rem;
            text-align: center;
        }

        /* ================= ALIENS EN NAVES ================= */
        .alien-layer {
            position: absolute;
            inset: 0;
            overflow: hidden;
            pointer-events: none;
            z-index: 1;
        }

        .alien-ship {
            position: absolute;
            font-size: 2.5rem;
            animation: fly 20s linear infinite;
            filter: drop-shadow(0 0 10px #00ffff);
            opacity: 0.9;
        }

        .alien-ship:nth-child(1) {
            top: 20%;
            left: -15%;
            animation-duration: 25s;
        }

        .alien-ship:nth-child(2) {
            top: 50%;
            left: -20%;
            animation-duration: 18s;
            font-size: 3rem;
        }

        .alien-ship:nth-child(3) {
            top: 75%;
            left: -25%;
            animation-duration: 30s;
            font-size: 2.2rem;
        }

        /* ================= ANIMACIÓN ================= */
        @keyframes fly {
            from {
                transform: translateX(0) rotate(0deg);
            }
            to {
                transform: translateX(130vw) rotate(360deg);
            }
        }
    </style>
</head>

<body>

<header class="header">

    <!-- ================= ALIENS EN NAVES ================= -->
    <div class="alien-layer">
        <div class="alien-ship">👽🛸</div>
        <div class="alien-ship">🛸👽</div>
        <div class="alien-ship">👾🛸</div>
    </div>

    <!-- ================= CONTENIDO ================= -->
    <div class="header-content">
        <h1>Aprendizaje Profesional con Inteligencia Artificial</h1>
        <p>La educación del futuro impulsada por tecnología avanzada y sistemas inteligentes</p>
        <a href="#contacto" class="btn-neon">Contactar</a>
    </div>

</header>

<section id="contacto" class="section">
    <h2>Contacto</h2>
    <p>Sumate a la nueva era del conocimiento.</p>
</section>

</body>
</html>
