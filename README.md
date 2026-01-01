<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Futuro IA</title>

<style>
/* ================= CONFIGURACIÓN GENERAL ================= */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, sans-serif;
}

body {
    background: radial-gradient(circle at top, #0a0020, #02010a 70%);
    color: #ffffff;
    overflow-x: hidden;
}

/* ================= HEADER ================= */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 60px;
    background: rgba(0,0,0,0.6);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(0,255,255,0.2);
}

.logo {
    font-size: 1.6rem;
    font-weight: bold;
    color: #00fff7;
    text-shadow: 0 0 15px #00fff7;
}

nav a {
    margin-left: 25px;
    text-decoration: none;
    color: #ffffff;
    position: relative;
    transition: 0.3s;
}

nav a::after {
    content: "";
    position: absolute;
    left: 0;
    bottom: -5px;
    width: 0%;
    height: 2px;
    background: linear-gradient(90deg, #00fff7, #a100ff);
    transition: 0.3s;
}

nav a:hover::after {
    width: 100%;
}

/* ================= HERO ================= */
.hero {
    min-height: 90vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 40px;
    background: linear-gradient(180deg, rgba(0,255,255,0.05), transparent);
}

.hero h1 {
    font-size: 3rem;
    background: linear-gradient(90deg, #00fff7, #b700ff);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-shadow: 0 0 25px rgba(183,0,255,0.5);
}

.hero p {
    margin: 20px 0 40px;
    font-size: 1.2rem;
    color: #cfcfcf;
}

.hero-buttons a {
    margin: 10px;
    padding: 15px 35px;
    border-radius: 30px;
    text-decoration: none;
    color: #fff;
    border: 2px solid #00fff7;
    box-shadow: 0 0 15px #00fff7;
    transition: 0.3s;
}

.hero-buttons a:hover {
    background: #00fff7;
    color: #000;
    box-shadow: 0 0 30px #00fff7;
}

/* ================= SECCIONES ================= */
section {
    padding: 80px 10%;
}

section h2 {
    font-size: 2.2rem;
    margin-bottom: 25px;
    text-align: center;
    color: #a100ff;
    text-shadow: 0 0 15px #a100ff;
}

section p {
    max-width: 900px;
    margin: auto;
    text-align: center;
    color: #d0d0d0;
    line-height: 1.7;
}

/* ================= CARDS ================= */
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 30px;
    margin-top: 50px;
}

.card {
    background: rgba(0,0,0,0.6);
    border: 1px solid rgba(0,255,255,0.4);
    border-radius: 20px;
    padding: 30px;
    text-align: center;
    box-shadow: 0 0 20px rgba(0,255,255,0.15);
    transition: 0.4s;
}

.card:hover {
    transform: translateY(-10px) scale(1.03);
    box-shadow: 0 0 40px rgba(161,0,255,0.6);
}

.card span {
    font-size: 2.5rem;
}

.card h3 {
    margin: 15px 0;
    color: #00fff7;
}

/* ================= CONTACTO ================= */
.contact {
    background: linear-gradient(180deg, transparent, rgba(161,0,255,0.15));
    border-top: 1px solid rgba(161,0,255,0.4);
}

.contact-box {
    max-width: 700px;
    margin: auto;
    background: rgba(0,0,0,0.7);
    border-radius: 25px;
    padding: 40px;
    box-shadow: 0 0 40px rgba(0,255,255,0.3);
    text-align: center;
}

.contact-box p {
    margin: 15px 0;
    font-size: 1.1rem;
}

.contact-buttons a {
    display: inline-block;
    margin: 10px;
    padding: 15px 30px;
    border-radius: 25px;
    text-decoration: none;
    border: 2px solid #a100ff;
    color: #fff;
    box-shadow: 0 0 15px #a100ff;
    transition: 0.3s;
}

.contact-buttons a:hover {
    background: #a100ff;
    box-shadow: 0 0 35px #a100ff;
}

/* ================= FOOTER ================= */
footer {
    text-align: center;
    padding: 25px;
    font-size: 0.9rem;
    color: #888;
}

/* ================= RESPONSIVE ================= */
@media (max-width: 768px) {
    header {
        flex-direction: column;
    }

    nav {
        margin-top: 15px;
    }

    .hero h1 {
        font-size: 2.3rem;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">🧠 Aprende IA</div>
    <nav>
        <a href="#">Inicio</a>
        <a href="#">Qué es la IA</a>
        <a href="#">Aprendizaje</a>
        <a href="#">Futuro</a>
        <a href="#">Contacto</a>
    </nav>
</header>

<section class="hero">
    <div>
        <h1>El Futuro de la Inteligencia Artificial Comienza Hoy</h1>
        <p>Humanos, máquinas y tecnología alienígena aprendiendo juntos.</p>
        <div class="hero-buttons">
            <a href="#">Contactarme</a>
            <a href="#">Más Información Académica</a>
        </div>
    </div>
</section>

<section>
    <h2>¿Qué Hacemos?</h2>
    <p>
        Enseñamos Inteligencia Artificial aplicada al mundo real, combinando tecnología humana
        con conceptos avanzados inspirados en sistemas inteligentes extraterrestres.
        Nuestro enfoque está orientado al aprendizaje del futuro: automatización,
        análisis de datos, machine learning y evolución digital.
    </p>
</section>

<section>
    <h2>Aprendizaje IA</h2>
    <div class="cards">
        <div class="card">
            <span>🤖</span>
            <h3>Machine Learning</h3>
            <p>Algoritmos que aprenden y evolucion
