
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aprendizaje de Inteligencia Artificial</title>
  <style>
    /* RESET CSS */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
    
    body {
      background: linear-gradient(to bottom, #0f2027, #203a43, #2c5364);
      color: #f0f0f0;
      line-height: 1.6;
    }

    header {
      background: #111;
      padding: 1rem;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 100;
      box-shadow: 0 2px 5px rgba(0,0,0,0.5);
    }

    header h1 {
      color: #00ffe7;
      font-size: 2rem;
      animation: glow 2s infinite alternate;
    }

    @keyframes glow {
      from { text-shadow: 0 0 5px #00ffe7; }
      to { text-shadow: 0 0 20px #00ffe7, 0 0 30px #00ffe7; }
    }

    nav {
      margin-top: 0.5rem;
    }

    nav a {
      color: #00ffe7;
      text-decoration: none;
      margin: 0 1rem;
      font-weight: bold;
      transition: 0.3s;
    }

    nav a:hover {
      color: #fff;
    }

    main {
      max-width: 1200px;
      margin: 2rem auto;
      padding: 0 1rem;
    }

    section {
      margin-bottom: 3rem;
    }

    h2 {
      color: #00ffe7;
      margin-bottom: 1rem;
      border-bottom: 2px solid #00ffe7;
      display: inline-block;
      padding-bottom: 0.3rem;
    }

    .card {
      background: rgba(255,255,255,0.05);
      padding: 1rem;
      border-radius: 10px;
      margin-bottom: 1rem;
      transition: transform 0.3s, background 0.3s;
    }

    .card:hover {
      transform: translateY(-5px);
      background: rgba(255,255,255,0.1);
    }

    .card img {
      max-width: 100%;
      border-radius: 10px;
      margin-bottom: 0.5rem;
    }

    .game {
      background: rgba(255,255,255,0.05);
      padding: 2rem;
      border-radius: 15px;
      text-align: center;
      position: relative;
    }

    .game h3 {
      color: #fffa00;
      margin-bottom: 1rem;
    }

    .options button {
      display: block;
      width: 100%;
      padding: 0.7rem;
      margin: 0.5rem 0;
      border: none;
      border-radius: 10px;
      background: #00ffe7;
      color: #000;
      font-weight: bold;
      cursor: pointer;
      transition: 0.3s;
    }

    .options button:hover {
      background: #00b8a9;
    }

    .feedback {
      margin-top: 1rem;
      font-weight: bold;
    }

    .score {
      margin-top: 1rem;
      font-size: 1.2rem;
      color: #fffa00;
    }

    footer {
      background: #111;
      padding: 1rem;
      text-align: center;
      margin-top: 2rem;
      color: #00ffe7;
    }

    .contact a {
      color: #00ffe7;
      margin: 0 0.5rem;
      text-decoration: none;
      font-weight: bold;
    }

    /* RESPONSIVE */
    @media(max-width:768px){
      nav a { display: block; margin: 0.5rem 0; }
    }
  </style>
</head>
<body>

  <header>
    <h1>Aprendizaje de Inteligencia Artificial 🧠</h1>
    <nav>
      <a href="#educacion">Educación</a>
      <a href="#juego">Juego Interactivo</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>

  <main>
    <!-- SECCIÓN EDUCATIVA -->
    <section id="educacion">
      <h2>Qué es la Inteligencia Artificial</h2>
      <div class="card">
        <p>La Inteligencia Artificial (IA) es una rama de la informática que busca crear sistemas capaces de realizar tareas que normalmente requieren inteligencia humana, como el aprendizaje, razonamiento y resolución de problemas.</p>
      </div>

      <h2>Python y Big Data en IA</h2>
      <div class="card">
        <p>Python es el lenguaje más usado para IA por su simplicidad y sus bibliotecas como TensorFlow y PyTorch. Big Data permite procesar grandes volúmenes de datos que son esenciales para entrenar modelos de IA.</p>
      </div>

      <h2>Aplicaciones actuales y futuras de IA</h2>
      <div class="card">
        <p>IA se usa en medicina, transporte, comercio, finanzas, biotecnología, y se proyecta que en el futuro estará presente en casi todos los sectores de la sociedad, optimizando procesos y creando nuevos servicios inteligentes.</p>
      </div>

      <h2>Impacto ambiental y social</h2>
      <div class="card">
        <p>El entrenamiento de modelos de IA consume energía y recursos. Además, la IA puede afectar empleos y privacidad, pero también ofrece soluciones para sostenibilidad, educación y salud.</p>
      </div>
    </section>

    <!-- SECCIÓN JUEGO -->
    <section id="juego">
      <h2>Juego Interactivo de IA</h2>
      <div class="game">
        <h3>Pregunta:</h3>
        <div class="question">Cargando pregunta...</div>
        <div class="options"></div>
        <div class="feedback"></div>
        <div class="score">Puntaje: 0</div>
        <button id="restart" style="margin-top:1rem; padding:0.5rem 1rem; border:none; border-radius:5px; cursor:pointer;">Reiniciar Juego</button>
      </div>
    </section>

    <!-- SECCIÓN CONTACTO -->
    <section id="contacto">
      <h2>Contacto</h2>
      <div class="card contact">
        <p>Teléfono: <a href="tel:+542235319300">2235319300</a></p>
        <p>Email: <a href="mailto:Donatoconturla100@gmail.com">Donatoconturla100@gmail.com</a></p>
        <p>Instagram: <a href="https://www.instagram.com/donatoacosta12/" target="_blank">@donatoacosta12</a></p>
        <p>WhatsApp: <a href="https://wa.me/542235319300" target="_blank">Enviar mensaje</a></p>
      </div>
    </section>
  </main>

  <footer>
    &copy; 2026 Aprendizaje de IA
  </footer>

  <script>
    // JUEGO DE PREGUNTAS
    const preguntas = [
      {
        pregunta: "¿Qué es la Inteligencia Artificial?",
        opciones: ["Un robot físico", "Programas que aprenden y razonan", "Una aplicación de dibujo", "Un lenguaje de programación"],
        correcta: 1,
        explicacion: "La IA consiste en programas capaces de aprender, razonar y tomar decisiones."
      },
      {
        pregunta: "¿Qué lenguaje se usa más en IA?",
        opciones: ["Python", "HTML", "CSS", "Coca-Cola"],
        correcta: 0,
        explicacion: "Python es ampliamente usado por sus bibliotecas y facilidad de uso."
      },
      {
        pregunta: "¿Qué es Big Data?",
        opciones: ["Conjunto de datos pequeños", "Una base de datos antigua", "Procesamiento de grandes volúmenes de datos", "Un juego de cartas"],
        correcta: 2,
        explicacion: "Big Data permite analizar grandes cantidades de información para tomar decisiones."
      },
      {
        pregunta: "Impacto ambiental de la IA:",
        opciones: ["Ninguno", "Consume energía y recursos", "Reduce la energía automáticamente", "No existe"],
        correcta: 1,
        explicacion: "Entrenar modelos de IA consume energía y recursos."
      }
    ];

    let indice = 0;
    let puntaje = 0;

    const questionEl = document.querySelector('.question');
    const optionsEl = document.querySelector('.options');
    const feedbackEl = document.querySelector('.feedback');
    const scoreEl = document.querySelector('.score');

    function cargarPregunta() {
      if(indice >= preguntas.length){
        questionEl.textContent = "¡Juego terminado!";
        optionsEl.innerHTML = "";
        feedbackEl.textContent = `Puntaje final: ${puntaje}`;
        return;
      }
      const q = preguntas[indice];
      questionEl.textContent = q.pregunta;
      optionsEl.innerHTML = "";
      feedbackEl.textContent = "";

      q.opciones.forEach((op, i)=>{
        const btn = document.createElement('button');
        btn.textContent = op;
        btn.onclick = ()=>verificarRespuesta(i);
        optionsEl.appendChild(btn);
      });
    }

    function verificarRespuesta(opcion){
      const q = preguntas[indice];
      if(opcion === q.correcta){
        feedbackEl.textContent = "✅ Correcto! " + q.explicacion;
        puntaje++;
      } else {
        feedbackEl.textContent = "❌ Incorrecto! " + q.explicacion;
      }
      scoreEl.textContent = "Puntaje: " + puntaje;
      indice++;
      setTimeout(cargarPregunta, 2000);
    }

    document.getElementById('restart').addEventListener('click', ()=>{
      indice = 0;
      puntaje = 0;
      scoreEl.textContent = "Puntaje: 0";
      cargarPregunta();
    });

    // Inicia juego
    cargarPregunta();
  </script>

</body>
</html>
