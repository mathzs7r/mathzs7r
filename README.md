<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Minhas Tecnologias</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      color: white;
      font-family: 'Segoe UI', system-ui, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      overflow-x: hidden;
    }

    h1 {
      font-size: 3.8rem;
      margin-bottom: 1.5rem;
      background: linear-gradient(90deg, #e66465, #9198e5, #4fd1c5);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-shadow: 0 0 30px rgba(255,255,255,0.2);
      animation: glow 3s ease-in-out infinite alternate;
    }

    .icons-container {
      display: flex;
      gap: 40px;
      flex-wrap: wrap;
      justify-content: center;
      padding: 40px;
    }

    .tech-icon {
      width: 110px;
      height: 110px;
      transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      filter: drop-shadow(0 10px 20px rgba(0,0,0,0.5));
      animation: float 6s ease-in-out infinite;
    }

    .tech-icon:hover {
      transform: translateY(-20px) scale(1.25) rotate(10deg);
      filter: drop-shadow(0 25px 40px rgba(255,255,255,0.25));
    }

    .tech-icon:nth-child(1) { animation-delay: 0.0s; }
    .tech-icon:nth-child(2) { animation-delay: 0.8s; }
    .tech-icon:nth-child(3) { animation-delay: 1.6s; }
    .tech-icon:nth-child(4) { animation-delay: 2.4s; }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50%      { transform: translateY(-25px); }
    }

    @keyframes glow {
      from { text-shadow: 0 0 20px rgba(255,100,100,0.5); }
      to   { text-shadow: 0 0 40px rgba(100,200,255,0.8); }
    }

    footer {
      margin-top: 80px;
      font-size: 1.1rem;
      opacity: 0.7;
    }
  </style>
</head>
<body>

  <h1>Minhas Tecnologias</h1>

  <div class="icons-container">
    <img 
      class="tech-icon"
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" 
      alt="HTML5" 
      title="HTML5"
    >
    <img 
      class="tech-icon"
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" 
      alt="CSS3" 
      title="CSS3"
    >
    <img 
      class="tech-icon"
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" 
      alt="JavaScript" 
      title="JavaScript"
    >
    <img 
      class="tech-icon"
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" 
      alt="Python" 
      title="Python"
    >
  </div>

  <footer>Made with ❤️ and a lot of coffee</footer>

</body>
</html>
