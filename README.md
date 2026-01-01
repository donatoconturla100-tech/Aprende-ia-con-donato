
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aprendizaje con Inteligencia Artificial</title>

    <!-- ================= CSS ORIGINAL ================= -->
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
    }

    /* ================= HEADER FUTURISTA ================= */
    .header {
        position: relative;
        height: 100vh;
        background: radial-gradient(circle at top, #1a0033, #000);
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
    }

    .header::before {
        content: "";
        position: absolute;
        width: 200%;
        height: 200%;
        background: url('https://www.transparenttextures.com/patterns/stardust.png');
        animation: moveStars 60s linear infinite;
    }

    @keyframes moveStars {
        from { transform: translateY(0); }
        to { transform: translateY(-1000px); }
    }

    .header-content {
        position: relative;
        text-align: center;
        z-index: 3;
        padding: 20px;
    }

    .header h1 {
        font-size: 3rem;
        color: #00ffff;
        text-shadow: 0 0 20px #00ffff;
    }

    .header p {
        margin: 20px 0;
        color: #bdbdff;
    }

    /* ================= BOTÓN NEÓN ================= */
    .btn-neon {
        display: inline-block;
        padding: 12px 30px;
        color: #00ffff;
        border: 2px solid #00ffff;
        text-decoration: none;
        border-radius: 30px;
        transition: 0.3s;
        box-shadow: 0 0 15px #00ffff;
    }

    .btn-neon:hover {
        background: #00ffff;
        color: #000;
        box-shadow: 0 0 30px #00ffff;
    }

    /* ================= ABOUT ================= */
    .about {
        padding: 60px 20px;
        text-align: center;
        background: linear-gradient(180deg, #000, #120022);
    }

    .about h2 {
        color: #7cff00;
        text-shadow: 0 0 10px #7cff00;
        margin-bottom: 20px;
    }

    /* ================= FEATURES ================= */
    .features {
        padding: 60px 20px;
        background: #070014;
    }

    .features h2 {
        text-align: center;
        color: #ff00ff;
        margin-bottom: 40px;
        text-shadow: 0 0 15px #ff00ff;
    }

    .cards {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
        gap: 25px;
    }

    .card {
        background: rgba(255,255,255,0.05);
        border: 1px solid #2b0055;
        border-radius: 15px;
        padding: 25px;
        text-align: center;
        transition: 0.3s;
    }

    .card span {
        font-size: 2.5rem;
    }

    .card:hover {
        transform: translateY(-10px);
        box-shadow: 0 0 25px #00ffff;
    }

    /* ================= VISUAL ================= */
    .visual {
        padding: 80px 20px;
        text-align: center;
        background: radial-gradient(circle, #120022, #000);
    }

    .space-animation {
        margin: 40px auto;
        width: 200px;
        height: 200px;
        border-radius: 50%;
        border: 2px solid #00ffff;
        box-shadow: 0 0 40px #00ffff;
        animation: pulse 3s infinite;
    }

    @keyframes pulse {
        0% { box-shadow: 0 0 20px #00ffff; }
        50% { box-shadow: 0 0 60px #7cff00; }
        100% { box-shadow: 0 0 20px #00ffff; }
    }

    /* ================= CONTACTO ================= */
    .contact {
        padding: 60px 20px;
        background: #05010d;
        text-align: center;
    }

    .contact h2 {
        color: #00ffff;
        margin-bottom: 20px;
    }

    /* ================= FOOTER ================= */
    footer {
        padding: 20px;
        text-align: center;
        background: #000;
        color: #777;
    }

    /* ================= RESPONSIVE ================= */
    @media (max-width: 768px) {
        .header h1 {
            font-size: 2rem;
        }
    }

    /* ========================================================= */
    /* === ALIENS ANIMADOS (AGREGADO) ========================== */
    /* ========================================================= */

    .alien-container {
        position: absolute;
        inset: 0;
        z-index: 2;
        pointer-events: none;
    }

    .alien {
        position: absolute;
        width: 80px;
        filter: drop-shadow(0 0 15px #00ffff);
        opacity: 0.9;
    }

    @keyframes alienDiagonal {
        from { transform: translate(-20%, 120%); }
        to { transform: translate(120%, -20%); }
    }

    @keyframes alienHorizontal {
        from { transform: translate(-30%, 30%); }
        to { transform: translate(120%, 30%); }
    }

    @keyframes alienZigzag {
        0% { transform: translate(-20%, 70%) rotate(0deg); }
        50% { transform: translate(50%, 60%) rotate(10deg); }
        100% { transform: translate(120%, 80%) rotate(-10deg); }
    }

    .alien.diagonal { animation: alienDiagonal 18s linear infinite; }
    .alien.horizontal { animation: alienHorizontal 25s linear infinite; }
    .alien.zigzag { animation: alienZigzag 22s linear infinite; }

    /* ========================================================= */
    /* === PERSONAJE FICTICIO DE FONDO (AGREGADO) =============== */
    /* ========================================================= */

    .character-container {
        position: absolute;
        bottom: 0;
        right: 5%;
        height: 90%;
        z-index: 1;
        pointer-events: none;
    }

    .character-image {
        height: 100%;
        max-height: 700px;
        object-fit: contain;
        opacity: 0.35;
        filter: grayscale(10%) contrast(1.05);
    }

    @media (max-width: 768px) {
        .character-container {
            right: 50%;
            transform: translateX(50%);
            opacity: 0.25;
        }
    }
    </style>
</head>

<body>

<!-- ================= HEADER FUTURISTA ================= -->
<header class="header">

    <!-- 👽 ALIENS -->
    <div class="alien-container">
        <img src="https://i.imgur.com/Z5pH2Xd.png" class="alien diagonal">
        <img src="https://i.imgur.com/Z5pH2Xd.png" class="alien horizontal">
        <img src="https://i.imgur.com/Z5pH2Xd.png" class="alien zigzag">
    </div>

    <!-- 🧍‍♂️ PERSONAJE FICTICIO -->
    <div class="character-container">
        <img src="TU_IMAGEN_AQUÍ.jpg" alt="Personaje ficticio" class="character-image">
    </div>

    <!-- CONTENIDO -->
    <div class="header-content">
        <h1>Aprendizaje Profesional con Inteligencia Artificial</h1>
        <p>La educación del futuro impulsada por tecnología avanzada y sistemas inteligentes</p>
        <a href="#contacto" class="btn-neon">Contactar</a>
    </div>
</header>

<section class="about">
    <h2>¿De qué trata?</h2>
    <p>Esta plataforma está diseñada para formar profesionales en Inteligencia Artificial, automatización y tecnologías del futuro.</p>
</section>

<section class="features">
    <h2>Tecnología del Futuro</h2>
    <div class="cards">
        <div class="card"><span>🤖</span><h3>IA Avanzada</h3></div>
        <div class="card"><span>🧠</span><h3>Aprendizaje Automático</h3></div>
        <div class="card"><span>🚀</span><h3>Naves Espaciales</h3></div>
        <div class="card"><span>🦾</span><h3>Robots</h3></div>
        <div class="card"><span>⚙️</span><h3>Sistemas Inteligentes</h3></div>
    </div>
</section>

<section class="visual">
    <h2>Explorando el Espacio Tecnológico</h2>
    <div class="space-animation"></div>
</section>

<section class="contact" id="contacto">
    <h2>Contacto</h2>
    <p>📧 Email: <strong>Donatoconturla100@gmail.com</strong></p>
    <p>📞 Teléfono: <strong>2235319300</strong></p>
</section>

<footer>
    <p>© 2025 • Tecnología del Futuro • Todos los derechos reservados</p>
</footer>

</body>
</html>
