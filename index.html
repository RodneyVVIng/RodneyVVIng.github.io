<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Te Amo Elizabeth</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      background: #ffeef5;
      overflow: hidden;
      font-family: 'Arial', sans-serif;
    }

    canvas {
      position: absolute;
      top: 0;
      left: 0;
      z-index: 0;
    }

    .center-button {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: #ff69b4;
      border: none;
      border-radius: 50px;
      width: 70px;
      height: 70px;
      cursor: pointer;
      z-index: 2;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
      outline: none;
      -webkit-tap-highlight-color: transparent;
    }

    .heart {
      width: 30px;
      height: 30px;
      background-color: #ffc0cb;
      position: relative;
      transform: rotate(-45deg);
    }

    .heart::before, .heart::after {
      content: "";
      width: 30px;
      height: 30px;
      background-color: #ffc0cb;
      border-radius: 50%;
      position: absolute;
    }

    .heart::before { top: -15px; left: 0; }
    .heart::after { top: 0; left: 15px; }

    .message {
      position: absolute;
      font-size: 1.2em;
      font-weight: bold;
      color: #d63384;
      z-index: 1;
      animation: glow 1.5s infinite alternate, floatUp 4s ease-out forwards;
      transform: translate(-50%, -50%);
      white-space: nowrap;
      opacity: 0;
    }

    @keyframes floatUp {
      0% { opacity: 0; transform: translate(-50%, -40%); }
      20% { opacity: 1; transform: translate(-50%, -50%); }
      100% { opacity: 0; transform: translate(-50%, -120%); }
    }

    @keyframes glow {
      0% { text-shadow: 0 0 5px #ff69b4, 0 0 10px #ff1493; }
      100% { text-shadow: 0 0 10px #ff1493, 0 0 20px #ff69b4; }
    }
  </style>
</head>
<body>
  <canvas id="cascade"></canvas>
  <button class="center-button" onclick="showMessage(event)">
    <div class="heart"></div>
  </button>

  <audio id="bg-music" loop autoplay>
    <source src="i-wanna-be-yours.mp3" type="audio/mpeg">
    Tu navegador no soporta audio HTML5.
  </audio>

  <script>
    // Configuración del fondo de emojis y textos
    const canvas = document.getElementById('cascade');
    const ctx = canvas.getContext('2d');
    let width = window.innerWidth;
    let height = window.innerHeight;
    canvas.width = width;
    canvas.height = height;

    const elements = ["🩷", "💖", "💗", "💕", "TE AMO", "TE AMO ELIZABETH"];
    const hearts = [];

    for (let i = 0; i < 50; i++) {
      hearts.push({
        x: Math.random() * width,
        y: Math.random() * height,
        size: 16 + Math.random() * 10,
        speed: 1 + Math.random() * 2,
        alpha: 0.6 + Math.random() * 0.4,
        text: elements[Math.floor(Math.random() * elements.length)]
      });
    }

    function drawCascade() {
      ctx.clearRect(0, 0, width, height);
      ctx.font = "20px Arial";
      hearts.forEach(h => {
        ctx.fillStyle = `rgba(255, 105, 180, ${h.alpha})`;
        ctx.fillText(h.text, h.x, h.y);
        h.y += h.speed;
        if (h.y > height) {
          h.y = -20;
          h.x = Math.random() * width;
        }
      });
      requestAnimationFrame(drawCascade);
    }

    drawCascade();
    window.addEventListener('resize', () => {
      width = window.innerWidth;
      height = window.innerHeight;
      canvas.width = width;
      canvas.height = height;
    });

    // Mensajes románticos con efecto de brillo
    const messages = [
      "Te amo Elizabeth", "Eres mi todo", "Mi muñequita hermosa",
      "Eres tan bonita", "Mi amor eterno", "Mi destino eres tú",
      "Cada día te amo más", "Mi única y verdadera", "Mi reina adorada",
      "Tú haces mi mundo más bonito", "Me haces tan feliz",
      "Te quiero mucho, chikis", "Te pienso siempre", "Mi corazón es tuyo"
    ];

    function showMessage(event) {
      event.preventDefault();
      if (navigator.vibrate) navigator.vibrate([100]);

      const msg = document.createElement('div');
      msg.classList.add('message');
      msg.textContent = messages[Math.floor(Math.random() * messages.length)];

      const btn = document.querySelector('.center-button');
      const btnRect = btn.getBoundingClientRect();

      const above = btnRect.top - 50 - Math.random() * 100;
      const below = btnRect.bottom + 50 + Math.random() * 100;

      const y = Math.random() < 0.5 ? above : below;
      const x = btnRect.left + btnRect.width / 2 + (Math.random() - 0.5) * 120;

      msg.style.left = `${x}px`;
      msg.style.top = `${y}px`;

      document.body.appendChild(msg);

      setTimeout(() => { msg.remove(); }, 4000);
    }

    // Autoplay fix para móviles
    window.addEventListener('click', () => {
      const music = document.getElementById('bg-music');
      if (music.paused) music.play().catch(() => {});
    }, { once: true });
  </script>
</body>
</html>
