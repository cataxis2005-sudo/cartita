<!doctype html>  
<html lang="es">  
<head>  
  <meta charset="utf-8" />  
  <meta name="viewport" content="width=device-width,initial-scale=1" />  
  <title>Para ti 💌</title>  
  <style>  
    * { box-sizing: border-box; margin: 0; padding: 0; }  
    body {  
      height: 100vh;  
      background: linear-gradient(180deg,#ffd6e0,#ffe8ec);  
      overflow: hidden;  
      display: flex;  
      align-items: center;  
      justify-content: center;  
      font-family: "Poppins", sans-serif;  
    }  
  
    .carta {  
      background: white;  
      padding: 2rem;  
      border-radius: 16px;  
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);  
      max-width: 500px;  
      text-align: center;  
      animation: aparecer 2s ease forwards;  
      opacity: 0;  
    }  
  
    .carta h1 {  
      color: #ff4d6d;  
      margin-bottom: 1rem;  
      font-size: 1.8rem;  
    }  
  
    .mensaje {  
      color: #444;  
      white-space: pre-wrap;  
      line-height: 1.6;  
      font-size: 1rem;  
    }  
  
    @keyframes aparecer {  
      from { transform: translateY(30px); opacity: 0; }  
      to { transform: translateY(0); opacity: 1; }  
    }  
  
    /* corazones flotando */  
    .heart {  
      position: absolute;  
      color: #ff4d6d;  
      font-size: 24px;  
      animation: floatUp linear forwards;  
      opacity: 0.8;  
    }  
  
    @keyframes floatUp {  
      0% { transform: translateY(0) scale(1); opacity: 1; }  
      100% { transform: translateY(-110vh) scale(1.4); opacity: 0; }  
    }  
  </style>  
</head>  
<body>  
  <div class="carta">  
    <h1>💌 Para ti 💌</h1>  
    <p class="mensaje">  
holis, mira la verdad me atraes muchísimo, llegaste en el momento en q huía del amor,   
y sinceramente me da miedo volver a amar, pero te lo quería decir porque mi corazón ya   
no puede más con todas las cosas que tengo, liberarme de esto ya sería algo menos.  
  
quizás yo ya no sea la persona que busques ni la que te interese,   
quizás si me pase de intensa y quería pedirte perdón por si te llego a molestar.  
  
yo con solo tener tu amistad soy feliz, pero en serio, yo no necesito a nadie,   
y si te digo esto es lo más puro que me ha salido del alma.  
  
perdóname por que me gustes, pero eres lo que anhelo en mi vida,   
no me importa lo que digan, tú para mí eres suficiente.  
  
espero que aun sabiendo esto sigas a mi lado como amigo,  
algún día se borrará este sentimiento que tengo.  
    </p>  
  </div>  
  
  <script>  
    // corazones flotando aleatoriamente  
    const body = document.body;  
  
    function crearCorazon() {  
      const heart = document.createElement('div');  
      heart.classList.add('heart');  
      heart.innerHTML = '❤️';  
      heart.style.left = Math.random() * 100 + 'vw';  
      heart.style.animationDuration = (4 + Math.random() * 3) + 's';  
      heart.style.fontSize = (18 + Math.random() * 12) + 'px';  
      body.appendChild(heart);  
      setTimeout(() => heart.remove(), 7000);  
    }  
  
    setInterval(crearCorazon, 400);  
  </script>  
</body>  
</html>  
