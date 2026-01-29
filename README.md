<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>RTOS + Pong | STM32F103</title>
  <style>
    :root {
      --primary: #00e5ff;
      --secondary: #1e1e2f;
      --accent: #ffcc00;
      --text: #eaeaea;
    }

    body {
      margin: 0;
      font-family: "Segoe UI", sans-serif;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      color: var(--text);
      line-height: 1.6;
    }

    header {
      text-align: center;
      padding: 3rem 1rem;
    }

    header h1 {
      font-size: 2.8rem;
      color: var(--primary);
      margin-bottom: 0.5rem;
    }

    header p {
      max-width: 700px;
      margin: auto;
      font-size: 1.1rem;
      opacity: 0.9;
    }

    section {
      max-width: 1000px;
      margin: auto;
      padding: 2rem 1rem;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
    }

    .card {
      background: rgba(255, 255, 255, 0.05);
      border-radius: 16px;
      padding: 1.5rem;
      backdrop-filter: blur(8px);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      cursor: pointer;
    }

    .card:hover {
      transform: translateY(-8px);
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.4);
    }

    .card h3 {
      color: var(--accent);
      margin-bottom: 0.5rem;
    }

    .tech-list span {
      display: inline-block;
      margin: 0.3rem;
      padding: 0.3rem 0.7rem;
      background: rgba(0, 229, 255, 0.15);
      border-radius: 20px;
      font-size: 0.85rem;
    }

    .button {
      display: inline-block;
      margin-top: 1.5rem;
      padding: 0.8rem 1.5rem;
      border-radius: 30px;
      background: var(--primary);
      color: #000;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s ease, transform 0.3s ease;
    }

    .button:hover {
      background: var(--accent);
      transform: scale(1.05);
    }

    footer {
      text-align: center;
      padding: 2rem;
      font-size: 0.9rem;
      opacity: 0.7;
    }

    /* Animación simple */
    .fade-in {
      animation: fade 1.2s ease forwards;
      opacity: 0;
    }

    @keyframes fade {
      to {
        opacity: 1;
      }
    }
  </style>
</head>

<body>

<header class="fade-in">
  <h1>RTOS + Pong en STM32F103</h1>
  <p>
    Sistema Operativo en Tiempo Real desarrollado para microcontroladores STM32,
    integrado con la lógica del clásico juego <strong>Pong</strong> y visualización
    en pantalla <strong>OLED</strong>.
  </p>
</header>

<section class="fade-in">
  <h2>🧠 Descripción del Proyecto</h2>
  <p>
    Este proyecto combina conceptos de <strong>sistemas embebidos</strong>,
    <strong>planificación en tiempo real</strong> y <strong>programación concurrente</strong>,
    demostrando cómo un RTOS puede gestionar múltiples tareas mientras ejecuta
    un videojuego clásico en hardware limitado.
  </p>
</section>

<section class="fade-in">
  <h2>⚙️ Características Principales</h2>
  <div class="cards">
    <div class="card">
      <h3>RTOS Embebido</h3>
      <p>
        Implementación de un sistema operativo en tiempo real con manejo de tareas,
        temporización y sincronización.
      </p>
    </div>

    <div class="card">
      <h3>Juego Pong</h3>
      <p>
        Lógica completa del juego Pong ejecutándose como tareas del RTOS,
        con control de colisiones y puntuación.
      </p>
    </div>

    <div class="card">
      <h3>Pantalla OLED</h3>
      <p>
        Visualización gráfica del juego en una pantalla OLED,
        optimizada para recursos limitados.
      </p>
    </div>

    <div class="card">
      <h3>STM32F103</h3>
      <p>
        Desarrollo orientado a microcontroladores ARM Cortex-M3,
        priorizando eficiencia y tiempo real.
      </p>
    </div>
  </div>
</section>

<section class="fade-in">
  <h2>🛠️ Tecnologías Utilizadas</h2>
  <div class="tech-list">
    <span>STM32F103</span>
    <span>C / Embedded C</span>
    <span>RTOS</span>
    <span>I2C / SPI</span>
    <span>Pantalla OLED</span>
    <span>Sistemas en Tiempo Real</span>
  </div>

  <a class="button" href="#" onclick="alert('Aquí puedes enlazar el repositorio o un video demo 🚀')">
    Ver Demo
  </a>
</section>

<footer>
  <p>Proyecto de Sistemas Embebidos · RTOS · STM32</p>
</footer>

</body>
</html>
