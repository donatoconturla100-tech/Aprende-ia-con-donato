<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Página Educativa + Juego IA</title>
  <style>
    /* ===================== */
    /* ESTILOS GENERALES */
    /* ===================== */
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to bottom, #0f0c29, #302b63, #24243e);
      color: #f0f0f0;
    }

    h1, h2, h3 {
      font-weight: 700;
    }

    a {
      text-decoration: none;
      color: #00ffe7;
    }

    /* ===================== */
    /* HEADER / NAVEGACIÓN */
    /* ===================== */
    header {
      background: rgba(0, 0, 0, 0.8);
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    header h1 {
      font-size: 1.5rem;
      color: #00ffe7;
    }

    nav a {
      margin-left: 20px;
      font-weight: 600;
      transition: 0.3s;
    }

    nav a:hover {
      color: #ff00ff;
    }

    /* ===================== */
    /* SECCIONES EDUCATIVAS */
    /* ===================== */
    section {
      padding: 50px 20px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .card {
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255,255,255,0.1);
      border-radius: 12px;
      padding: 20px;
      transition: transform 0.3s, box-shadow 0.3s;
      position: relative;
      overflow: hidden;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 0 20px rgba(0,255,231,0.3);
    }

    .card h3 {
      margin-top: 0;
      color: #00ffe7;
    }

    .card p {
      line-height: 1.5;
      font-size: 0.95rem;
    }

    /* Decoraciones futuristas con CSS */
    .card::before {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(0,255,231,0.05) 1%, transparent 1%) center/20px 20px;
      pointer-events: none;
    }

    /* ===================== */
    /* JUEGO INTERACTIVO */
    /* ===================== */
    #game-section {
      background: linear-gradient(to bottom right, #0f0c29, #1f1b3a);
      padding: 50px 20px;
    }

    #game {
      max-width: 700px;
      margin: 0 auto;
      background: rgba(255,255,255,0.05);
      border-radius: 12px;
      padding: 30px;
      text-align: center;
      box-shadow: 0 0 20px rgba(0,255,231,0.2);
    }

    #question {
      font-size: 1.2rem;
      margin-bottom: 20px;
    }

    .options {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .option-btn {
      background: rgba(0,255,231,0.1);
      border: 1px solid #00ffe7;
      border-radius: 8px;
      padding: 12px;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
    }

    .option-btn:hover {
      background: rgba(0,255,231,0.2);
      transform: translateX(5px);
    }

    .feedback {
      margin-top: 20px;
      font-weight: 600;
      min-height: 30px;
    }

    #score {
      margin-top: 15px;
      font-size: 1rem;
      color: #ffea00;
    }

    #restart {
      margin-top: 20px;
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      background: #ff00ff;
      color: #fff;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
    }

    #restart:hover {
      background: #ff4fff;
    }

    /* ===================== */
    /* RESPONSIVE */
    /* ===================== */
    @media(max-width: 768px){
      header {
        flex-direction: column;
        align-items: flex-start;
      }

      nav {
        margin-top: 10px;
      }
    }
  </style>
</head>
<body>

  <!-- ===================== -->
  <!-- HEADER / NAVEGACIÓN -->
  <!-- ===================== -->
  <header>
    <h1>Explora IA</h1>
    <nav>
      <a href="#edu-section">Educación</a>
      <a href="#game-section">Juego</a>
    </nav>
  </header>

  <!-- ===================== -->
  <!-- SECCIÓN EDUCATIVA -->
  <!-- ===================== -->
  <section id="edu-section">
    <h2>Aprende sobre Inteligencia Artificial</h2>
    <div class="cards">

      <div class="card">
        <h3>¿Qué es la Inteligencia Artificial?</h3>
        <p>La Inteligencia Artificial (IA) es una rama de la informática que busca crear sistemas capaces de realizar tareas que normalmente requieren inteligencia humana, como reconocimiento de voz, aprendizaje y toma de decisiones.</p>
      </div>

      <div class="card">
        <h3>Python y Big Data en IA</h3>
        <p>Python es uno de los lenguajes más usados en IA por su simplicidad y poderosas librerías. Big Data permite analizar grandes volúmenes de información, esencial para entrenar modelos de IA.</p>
      </div>

      <div class="card">
        <h3>Aplicaciones actuales y futuras</h3>
        <p>La IA se aplica en medicina, finanzas, transporte, educación y entretenimiento. Futuras aplicaciones incluyen asistencia personalizada, ciudades inteligentes y predicción de problemas globales.</p>
      </div>

      <div class="card">
        <h3>Impacto ambiental y social</h3>
        <p>La IA consume energía y recursos, lo que genera impacto ambiental. Socialmente, mejora la eficiencia y crea nuevas oportunidades laborales, pero también plantea desafíos éticos y de privacidad.</p>
      </div>

    </div>
  </section>

  <!-- ===================== -->
  <!-- SECCIÓN DEL JUEGO -->
  <!-- ===================== -->
  <section id="game-section">
    <h2>Juego Interactivo de Preguntas sobre IA</h2>
    <div id="game">
      <div id="question">Pregunta cargando...</div>
      <div class="options" id="options"></div>
      <div class="feedback" id="feedback"></div>
      <div id="score">Puntaje: 0</div>
      <button id="restart">Reiniciar Juego</button>
    </div>
  </section>

  <!-- ===================== -->
  <!-- JAVASCRIPT -->
  <!-- ===================== -->
  <script>
    // =====================
    // DATOS DEL JUEGO
    // =====================
    const questions = [
      {
        question: "¿En qué año se considera que comenzó la IA como campo académico?",
        options: ["1956", "1945", "1969", "1972"],
        answer: 0,
        explanation: "La conferencia de Dartmouth en 1956 marcó el inicio formal de la IA."
      },
      {
        question: "¿Cuál de estas librerías de Python se usa para Machine Learning?",
        options: ["NumPy", "Pandas", "Scikit-learn", "Matplotlib"],
        answer: 2,
        explanation: "Scikit-learn es la librería más usada para algoritmos de Machine Learning."
      },
      {
        question: "¿Qué es Big Data?",
        options: ["Un tipo de IA", "Grandes volúmenes de datos", "Un lenguaje de programación", "Un robot"],
        answer: 1,
        explanation: "Big Data se refiere al procesamiento y análisis de grandes volúmenes de datos."
      },
      {
        question: "¿Qué impacto ambiental puede generar la IA?",
        options: ["Ninguno", "Consumo energético alto", "Solo reciclaje", "Contaminación acústica"],
        answer: 1,
        explanation: "El entrenamiento de modelos de IA consume energía, contribuyendo al impacto ambiental."
      },
      {
        question: "Python es popular en IA por:",
        options: ["Ser rápido como C++", "Simplicidad y librerías", "Tener GUI avanzada", "Ser usado en videojuegos"],
        answer: 1,
        explanation: "Python combina facilidad de uso con librerías potentes, ideal para IA."
      }
    ];

    // =====================
    // VARIABLES
    // =====================
    let currentQuestion = 0;
    let score = 0;

    const questionEl = document.getElementById("question");
    const optionsEl = document.getElementById("options");
    const feedbackEl = document.getElementById("feedback");
    const scoreEl = document.getElementById("score");
    const restartBtn = document.getElementById("restart");

    // =====================
    // FUNCIONES DEL JUEGO
    // =====================
    function loadQuestion() {
      feedbackEl.textContent = "";
      if(currentQuestion >= questions.length){
        questionEl.textContent = "¡Juego terminado!";
        optionsEl.innerHTML = "";
        feedbackEl.textContent = `Tu puntaje final es ${score} / ${questions.length}`;
        return;
      }
      const q = questions[currentQuestion];
      questionEl.textContent = q.question;

      optionsEl.innerHTML = "";
      q.options.forEach((opt, index) => {
        const btn = document.createElement("button");
        btn.className = "option-btn";
        btn.textContent = opt;
        btn.onclick = () => checkAnswer(index);
        optionsEl.appendChild(btn);
      });
    }

    function checkAnswer(selected) {
      const q = questions[currentQuestion];
      if(selected === q.answer){
        feedbackEl.textContent = "✅ Correcto: " + q.explanation;
        score++;
      } else {
        feedbackEl.textContent = "❌ Incorrecto: " + q.explanation;
      }
      scoreEl.textContent = `Puntaje: ${score}`;
      currentQuestion++;
      setTimeout(loadQuestion, 2000);
    }

    function restartGame() {
      currentQuestion = 0;
      score = 0;
      scoreEl.textContent = `Puntaje: ${score}`;
      loadQuestion();
    }

    // =====================
    // EVENTOS
    // =====================
    restartBtn.addEventListener("click", restartGame);

    // Cargar primera pregunta
    loadQuestion();
  </script>
</body>
</html>
