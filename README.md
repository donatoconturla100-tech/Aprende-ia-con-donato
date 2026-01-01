<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Era Artificial – Aprende y Domina la IA</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* ================== Reset y tipografía ================== */
    * { margin:0; padding:0; box-sizing:border-box; }
    body {
      font-family: 'Orbitron', sans-serif;
      background: #0d0d0d;
      color: #fff;
      overflow-x: hidden;
    }
    a { text-decoration: none; color: inherit; }
    button { cursor: pointer; font-family: inherit; }

    /* ================== Fondo futurista con partículas ================== */
    #particles {
      position: fixed;
      top:0; left:0;
      width:100%; height:100%;
      z-index: -1;
    }

    /* ================== Header ================== */
    header {
      text-align: center;
      padding: 50px 20px 30px;
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
    }
    header h1 {
      font-size: 2.5rem;
      color: #0ff;
      text-shadow: 0 0 10px #0ff, 0 0 20px #0ff;
      margin-bottom: 10px;
    }

    /* ================== Secciones ================== */
    section {
      padding: 50px 20px;
      max-width: 1000px;
      margin: 0 auto;
      transition: all 0.3s ease;
    }
    section h2 {
      font-size: 2rem;
      color: #8a2be2;
      text-shadow: 0 0 5px #8a2be2, 0 0 15px #00f0ff;
      margin-bottom: 20px;
    }
    section p {
      font-size: 1rem;
      line-height: 1.6;
      color: #ccc;
    }
    .expandable {
      max-height: 100px;
      overflow: hidden;
      transition: max-height 0.5s ease;
    }
    .expandable.show {
      max-height: 1000px;
    }
    .btn-expand {
      display: inline-block;
      margin-top: 10px;
      background: #0ff;
      color: #000;
      padding: 8px 15px;
      border-radius: 5px;
      font-weight: bold;
      transition: all 0.3s ease;
    }
    .btn-expand:hover {
      background: #8a2be2;
      color: #fff;
      box-shadow: 0 0 15px #8a2be2, 0 0 25px #0ff;
    }

    /* ================== Chatbot ================== */
    #chatbot {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #111;
      border: 2px solid #0ff;
      border-radius: 10px;
      width: 300px;
      max-width: 90%;
      padding: 10px;
      box-shadow: 0 0 20px #0ff;
    }
    #chatbot h3 {
      text-align: center;
      margin-bottom: 10px;
      color: #0ff;
      text-shadow: 0 0 5px #0ff;
    }
    #chatbot-messages {
      height: 200px;
      overflow-y: auto;
      border: 1px solid #0ff;
      padding: 5px;
      margin-bottom: 10px;
      background: #000;
    }
    #chatbot input {
      width: calc(100% - 50px);
      padding: 5px;
      border-radius: 5px;
      border: 1px solid #0ff;
      background: #111;
      color: #fff;
    }
    #chatbot button {
      width: 40px;
      background: #0ff;
      border: none;
      border-radius: 5px;
      font-weight: bold;
      transition: all 0.3s ease;
    }
    #chatbot button:hover {
      background: #8a2be2;
      color: #fff;
      box-shadow: 0 0 10px #8a2be2;
    }

    /* ================== Contactos ================== */
    .contact-links {
      margin-top: 20px;
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
    }
    .contact-links a {
      background: #0ff;
      color: #000;
      padding: 10px 15px;
      border-radius: 8px;
      font-weight: bold;
      transition: all 0.3s ease;
    }
    .contact-links a:hover {
      background: #8a2be2;
      color: #fff;
      box-shadow: 0 0 15px #8a2be2;
    }

    /* ================== Footer ================== */
    footer {
      text-align: center;
      padding: 30px 20px;
      background: #111;
      color: #0ff;
      text-shadow: 0 0 5px #0ff;
    }

    /* ================== Responsive ================== */
    @media (max-width:768px){
      header h1 { font-size:2rem; }
      section { padding: 30px 15px; }
    }

  </style>
</head>
<body>
  <!-- Partículas de fondo -->
  <canvas id="particles"></canvas>

  <!-- Header -->
  <header>
    <h1>Era Artificial – Aprende y Domina la IA</h1>
  </header>

  <!-- Secciones -->
  <section id="sobre-nosotros">
    <h2>Sobre nosotros</h2>
    <p>En la Era Artificial nos dedicamos a enseñar a ser protagonistas de nuestra propia historia, llevando tus ideas al siguiente nivel. No todo es solo prompt en IA; aprender a usarla correctamente y adaptarla a nuestra vida diaria es nuestra misión.</p>
  </section>

  <section id="historia-ia">
    <h2>Historia de la IA</h2>
    <div class="expandable" id="historia-expand">
      <p>La inteligencia artificial ha evolucionado desde simples programas de cálculo hasta complejas redes neuronales capaces de aprender y generar contenido creativo. Su impacto social y cultural es profundo, transformando industrias, educación y la forma en que interactuamos con la tecnología. Adaptarla a la vida real implica comprender sus posibilidades y limitaciones, y usarla éticamente para mejorar nuestras decisiones y procesos diarios.</p>
    </div>
    <button class="btn-expand" onclick="toggleExpandable('historia-expand')">Leer más</button>
  </section>

  <section id="aprendizaje-practico">
    <h2>Aprendizaje práctico</h2>
    <div class="expandable" id="aprendizaje-expand">
      <p>En esta sección aprenderás sobre prompts, ejemplos de uso de IA y consejos para aplicar la inteligencia artificial de manera ética y efectiva. La IA puede ayudarte a generar ideas, optimizar tareas y resolver problemas complejos. Usando prompts claros y éticos, podrás obtener resultados sorprendentes y útiles en tu vida académica y profesional.</p>
    </div>
    <button class="btn-expand" onclick="toggleExpandable('aprendizaje-expand')">Leer más</button>
  </section>

  <section id="contacto">
    <h2>Contacto y redes sociales</h2>
    <p>Teléfono: 2235319300</p>
    <p>Correo: <a href="mailto:Donatoconturla100@gmail.com">Donatoconturla100@gmail.com</a></p>
    <p>Instagram: <a href="https://www.instagram.com/donatoacosta12/" target="_blank">@donatoacosta12</a></p>
    <div class="contact-links">
      <a href="https://wa.me/5492235319300?text=Hola,%20quiero%20contactarte%20sobre%20la%20IA" target="_blank">WhatsApp</a>
      <a href="https://www.instagram.com/donatoacosta12/" target="_blank">Instagram</a>
      <a href="mailto:Donatoconturla100@gmail.com">Correo</a>
    </div>
  </section>

  <!-- Chatbot -->
  <div id="chatbot">
    <h3>Chat IA</h3>
    <div id="chatbot-messages"></div>
    <input type="text" id="chatbot-input" placeholder="Escribe tu pregunta...">
    <button onclick="sendMessage()">➤</button>
  </div>

  <!-- Footer -->
  <footer>
    <p>Teléfono: 2235319300 | Correo: Donatoconturla100@gmail.com</p>
    <p>© 2026 Era Artificial. Todos los derechos reservados.</p>
    <p>Aprende, crea y transforma tu mundo con IA.</p>
  </footer>

  <!-- ================== JavaScript ================== -->
  <script>
    // Expandable sections
    function toggleExpandable(id){
      const el = document.getElementById(id);
      el.classList.toggle('show');
    }

    // Chatbot básico
    const chatbotMessages = document.getElementById('chatbot-messages');
    const chatbotInput = document.getElementById('chatbot-input');

    const faq = {
      "qué es la ia": "La IA es la simulación de procesos inteligentes por parte de máquinas. Aquí aprenderás cómo usarla y aplicarla.",
      "cómo usar la ia": "Puedes usar la IA mediante prompts claros y aplicando sus resultados de manera ética en la vida real.",
      "qué son los prompts": "Los prompts son instrucciones o preguntas que le das a la IA para generar respuestas o soluciones.",
      "para qué sirve esta página": "Esta página te enseña a aprender, usar y comprender la IA, su historia y aplicaciones prácticas."
    };

    function sendMessage(){
      const text = chatbotInput.value.trim().toLowerCase();
      if(!text) return;
      appendMessage("Tú: " + chatbotInput.value);
      let response = "Lo siento, no entendí tu pregunta. Intenta con algo más específico sobre IA.";
      for(let key in faq){
        if(text.includes(key)){
          response = faq[key];
          break;
        }
      }
      setTimeout(()=>{ appendMessage("IA: " + response); }, 500);
      chatbotInput.value = "";
    }

    function appendMessage(msg){
      const p = document.createElement('p');
      p.textContent = msg;
      chatbotMessages.appendChild(p);
      chatbotMessages.scrollTop = chatbotMessages.scrollHeight;
    }

    // Partículas estilo red neuronal
    const canvas = document.getElementById('particles');
    const ctx = canvas.getContext('2d');
    let particlesArray = [];
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

    window.addEventListener('resize', () => {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
      initParticles();
    });

    class Particle {
      constructor(){
        this.x = Math.random() * canvas.width;
        this.y = Math.random() * canvas.height;
        this.size = Math.random() * 2 + 1;
        this.speedX = Math.random() * 1 - 0.5;
        this.speedY = Math.random() * 1 - 0.5;
      }
      update(){
        this.x += this.speedX;
        this.y += this.speedY;
        if(this.x < 0 || this.x > canvas.width) this.speedX *= -1;
        if(this.y < 0 || this.y > canvas.height) this.speedY *= -1;
      }
      draw(){
        ctx.fillStyle = '#0ff';
        ctx.beginPath();
        ctx.arc(this.x, this.y, this.size, 0, Math.PI*2);
        ctx.fill();
      }
    }

    function initParticles(){
      particlesArray = [];
      for(let i=0;i<100;i++){
        particlesArray.push(new Particle());
      }
    }

    function connectParticles(){
      for(let a=0;a<particlesArray.length;a++){
        for(let b=a;b<particlesArray.length;b++){
          let dx = particlesArray[a].x - particlesArray[b].x;
          let dy = particlesArray[a].y - particlesArray[b].y;
          let distance = Math.sqrt(dx*dx + dy*dy);
          if(distance < 100){
            ctx.strokeStyle = 'rgba(0,255,255,' + (1 - distance/100) + ')';
            ctx.lineWidth = 1;
            ctx.beginPath();
            ctx.moveTo(particlesArray[a].x, particlesArray[a].y);
            ctx.lineTo(particlesArray[b].x, particlesArray[b].y);
            ctx.stroke();
          }
        }
      }
    }

    function animateParticles(){
      ctx.clearRect(0,0,canvas.width,canvas.height);
      particlesArray.forEach(p => { p.update(); p.draw(); });
      connectParticles();
      requestAnimationFrame(animateParticles);
    }

    initParticles();
    animateParticles();
  </script>
</body>
</html>
