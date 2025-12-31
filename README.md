<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aprendizaje con Inteligencia Artificial</title>

    <!-- Enlace al archivo de estilos -->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- ================= HEADER FUTURISTA ================= -->
    <header class="header">
        <div class="overlay"></div>
        <div class="header-content">
            <h1>Aprendizaje Profesional con Inteligencia Artificial</h1>
            <p>La educación del futuro impulsada por tecnología avanzada y sistemas inteligentes</p>
            <a href="#contacto" class="btn-neon">Contactar</a>
        </div>
    </header>

    <!-- ================= SECCIÓN DE QUÉ TRATA ================= -->
    <section class="about">
        <h2>¿De qué trata?</h2>
        <p>
            Esta plataforma está diseñada para formar profesionales en Inteligencia Artificial,
            automatización y tecnologías del futuro. Aprendé a dominar sistemas inteligentes,
            innovación tecnológica y soluciones avanzadas que están transformando el mundo.
        </p>
    </section>

    <!-- ================= SECCIÓN CARACTERÍSTICAS ================= -->
    <section class="features">
        <h2>Tecnología del Futuro</h2>

        <div class="cards">
            <div class="card">
                <span>🤖</span>
                <h3>IA Avanzada</h3>
                <p>Sistemas inteligentes capaces de aprender y evolucionar.</p>
            </div>

            <div class="card">
                <span>🧠</span>
                <h3>Aprendizaje Automático</h3>
                <p>Modelos que mejoran su rendimiento con datos.</p>
            </div>

            <div class="card">
                <span>🚀</span>
                <h3>Naves Espaciales</h3>
                <p>Inspiración en tecnología aeroespacial del futuro.</p>
            </div>

            <div class="card">
                <span>🦾</span>
                <h3>Robots</h3>
                <p>Automatización avanzada y robótica inteligente.</p>
            </div>

            <div class="card">
                <span>⚙️</span>
                <h3>Sistemas Inteligentes</h3>
                <p>Infraestructuras tecnológicas autónomas.</p>
            </div>
        </div>
    </section>

    <!-- ================= SECCIÓN VISUAL FUTURISTA ================= -->
    <section class="visual">
        <h2>Explorando el Espacio Tecnológico</h2>
        <p>
            Un entorno visual inspirado en el espacio, máquinas futuristas
            y la evolución de la inteligencia artificial.
        </p>
        <div class="space-animation"></div>
    </section>

    <!-- ================= SECCIÓN CONTACTO ================= -->
    <section class="contact" id="contacto">
        <h2>Contacto</h2>
        <p>📧 Email: <strong>Donatoconturla100@gmail.com</strong></p>
        <p>📞 Teléfono: <strong>2235319300</strong></p>
    </section>

    <!-- ================= FOOTER ================= -->
    <footer>
        <p>© 2025 • Tecnología del Futuro • Todos los derechos reservados</p>
    </footer>

</body>
</html>
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
    z-index: 1;
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

/* ================= SECCIÓN ABOUT ================= */
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
    background: rgba(255, 255, 255, 0.05);
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

/* ================= SECCIÓN VISUAL ================= */
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
