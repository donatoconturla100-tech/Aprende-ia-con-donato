
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aprendizaje de IA | Futuro Tecnológico</title>

<style>
/* ================= RESET ================= */
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Segoe UI', Tahoma, sans-serif;
}

/* ================= BODY ================= */
body{
    background: radial-gradient(circle at top, #0b0220, #02000a 70%);
    color:#eaeaff;
    overflow-x:hidden;
}

/* ================= HEADER ================= */
header{
    padding:60px 20px;
    text-align:center;
}

header h1{
    font-size:3rem;
    color:#7df9ff;
    text-shadow:0 0 20px #00f0ff;
    animation: glow 3s infinite alternate;
}

header p{
    max-width:800px;
    margin:20px auto 0;
    color:#cfcfff;
}

/* ================= SECTIONS ================= */
section{
    padding:80px 10%;
    position:relative;
}

section h2{
    font-size:2.2rem;
    color:#b98cff;
    margin-bottom:20px;
}

section p, section li{
    line-height:1.7;
    color:#ddddff;
}

ul{
    margin-left:20px;
}

/* ================= FUTURISTIC DIVIDER ================= */
.divider{
    height:2px;
    background:linear-gradient(90deg, transparent, #7df9ff, transparent);
    margin:60px 0;
}

/* ================= ALIENS & ROBOTS ================= */
.alien, .robot{
    position:absolute;
    width:60px;
    height:60px;
    border-radius:50%;
    filter:drop-shadow(0 0 10px #00f0ff);
}

.alien{
    background:radial-gradient(circle, #00ffcc, #006666);
    animation: floatAlien 12s linear infinite;
}

.robot{
    background:linear-gradient(135deg, #999, #444);
    border-radius:10px;
    animation: walkRobot 10s linear infinite;
}

.alien::after{
    content:'';
    position:absolute;
    top:15px;
    left:15px;
    width:8px;
    height:8px;
    background:#000;
    border-radius:50%;
    box-shadow:20px 0 #000;
}

.robot::after{
    content:'';
    position:absolute;
    bottom:-10px;
    left:10px;
    width:40px;
    height:10px;
    background:#222;
}

/* ================= CONTACT ================= */
.contact{
    text-align:center;
    padding:80px 20px;
}

.buttons{
    display:flex;
    justify-content:center;
    gap:25px;
    flex-wrap:wrap;
}

.btn{
    padding:15px 30px;
    border-radius:40px;
    text-decoration:none;
    color:#fff;
    font-weight:bold;
    background:linear-gradient(135deg, #6a00ff, #00f0ff);
    box-shadow:0 0 20px rgba(0,240,255,.6);
    transition:all .4s ease;
}

.btn:hover{
    transform:scale(1.1);
    box-shadow:0 0 35px #7df9ff;
}

/* ================= FOOTER ================= */
footer{
    text-align:center;
    padding:30px;
    color:#888;
    font-size:.9rem;
}

/* ================= ANIMATIONS ================= */
@keyframes glow{
    from{ text-shadow:0 0 10px #00f0ff; }
    to{ text-shadow:0 0 30px #7df9ff; }
}

@keyframes floatAlien{
    0%{ left:-10%; top:20%; }
    100%{ left:110%; top:40%; }
}

@keyframes walkRobot{
    0%{ right:-10%; bottom:10%; }
    100%{ right:110%; bottom:15%; }
}
</style>
</head>

<body>

<header>
    <h1>Aprendizaje del Futuro</h1>
    <p>Exploramos la Inteligencia Artificial y la Programación como pilares de la tecnología avanzada del mañana.</p>
</header>

<div class="alien"></div>
<div class="robot"></div>

<section>
    <h2>🧠 Aprendizaje de Inteligencia Artificial</h2>
    <p>
        El aprendizaje de Inteligencia Artificial es el proceso mediante el cual las máquinas adquieren la capacidad
        de analizar datos, aprender patrones y tomar decisiones inteligentes sin intervención humana constante.
    </p>
    <ul>
        <li>Aprendizaje supervisado</li>
        <li>Aprendizaje no supervisado</li>
        <li>Aprendizaje profundo (Deep Learning)</li>
        <li>Redes neuronales artificiales</li>
    </ul>
    <p>
        La IA se aplica en medicina, robótica, finanzas, automatización, análisis de datos y exploración espacial,
        permitiendo un futuro más eficiente, inteligente y conectado.
    </p>
</section>

<div class="divider"></div>

<section>
    <h2>💻 Aprendizaje de Programación</h2>
    <p>
        La programación es la base del mundo digital. Aprender a programar desarrolla la lógica, el pensamiento crítico
        y la capacidad de crear soluciones tecnológicas reales.
    </p>
    <ul>
        <li>Fundamentos de programación</li>
        <li>Introducción a Python</li>
        <li>Lógica y estructuras de control</li>
        <li>Automatización y análisis de datos</li>
    </ul>
    <p>
        Python es uno de los lenguajes más usados en Inteligencia Artificial por su simplicidad, potencia y versatilidad,
        siendo clave en el desarrollo de sistemas inteligentes.
    </p>
</section>

<div class="divider"></div>

<section class="contact">
    <h2>📡 Contacto Futurista</h2>
    <div class="buttons">
        <a class="btn" href="https://wa.me/2235319300" target="_blank">WhatsApp</a>
        <a class="btn" href="https://www.instagram.com/donato%20acosta%2012/" target="_blank">Instagram</a>
        <a class="btn" href="mailto:donatoconturla100@gmail.com">Gmail</a>
    </div>
</section>

<footer>
    © Futuro IA · Tecnología Avanzada · Diseño Futurista
</footer>

</body>
</html>
