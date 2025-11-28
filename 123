<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>New Year Surprise 🎉</title>
<style>
  body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(135deg, #ffdde1, #ee9ca7);
    overflow: hidden;
    position: relative;
  }

  .screen {
    display: none;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    padding: 20px;
    gap: 20px;
    opacity: 0;
    transform: scale(0.9);
    transition: all 0.6s ease;
    position: relative;
    z-index: 2;
    text-align: center;
  }
  .active { display: flex; opacity: 1; transform: scale(1); }

  .shinchan {
    width: 150px;
    height: auto;
    animation: float 2s ease-in-out infinite alternate;
  }

  @keyframes float {
    from { transform: translateY(0); }
    to { transform: translateY(-15px); }
  }

  .text-container {
    max-width: 500px;
  }

  h1 { font-size: 1.8rem; margin-bottom: 10px; color: #ff4081; }
  p { font-size: 1.1rem; margin-bottom: 10px; color: #444; }

  button {
    padding: 10px 20px;
    border: none;
    border-radius: 12px;
    background: #ff69b4;
    color: white;
    cursor: pointer;
    margin: 5px;
    font-size: 1rem;
    transition: 0.3s;
  }
  button:hover { transform: scale(1.1); box-shadow: 0 0 15px rgba(255,105,180,0.6); }

  /* Floating hearts */
  .heart {
    position: fixed;
    bottom: -10px;
    color: red;
    font-size: 20px;
    animation: floatUp 5s linear infinite;
    z-index: 1;
  }
  @keyframes floatUp {
    from { transform: translateY(0) scale(1); opacity: 1; }
    to { transform: translateY(-110vh) scale(1.5); opacity: 0; }
  }

  /* Fireworks canvas */
  canvas#fireworks {
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    z-index: 0;
    pointer-events: none;
    background: transparent;
  }

  /* Memories */
  .memories-img {
    width: 70%;
    border-radius: 15px;
    box-shadow: 0 0 15px rgba(0,0,0,0.2);
    transition: transform 0.6s ease, opacity 0.6s ease;
  }

  .slide-in-right { transform: translateX(100%); opacity: 0; }
  .slide-in-left { transform: translateX(-100%); opacity: 0; }
  .slide-active { transform: translateX(0); opacity: 1; }
</style>
</head>
<body>

<canvas id="fireworks"></canvas>
<div id="heart-container"></div>

<!-- PAGE 1 -->
<div id="screen1" class="screen active">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>🎉 Happy New Year, Sis 💖</h1>
    <p>May this year be full of smiles, peace, and laughter!</p>
    <button onclick="showScreen('like')">Next</button>
  </div>
</div>

<!-- PAGE 2 -->
<div id="screenLike" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>Do you like me? 💖</h1>
    <button onclick="showScreen('goodGirl')">Yes</button>
    <button onclick="showScreen('please')">No</button>
  </div>
</div>

<!-- NEW PAGE after YES -->
<div id="screenGoodGirl" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>😄 I thought you might click No!</h1>
    <p>Good girl 💖 You actually clicked Yes — I'm proud of you!</p>
    <button onclick="showScreen('thank')">Next</button>
  </div>
</div>

<!-- PAGE 3 -->
<div id="screenPlease" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>Please, my cute bestie! 😘</h1>
    <p>Click Yes! I promise a special message is waiting for you! 🎉</p>
    <button onclick="showScreen('thank')">Yes</button>
  </div>
</div>

<!-- PAGE 4 -->
<div id="screenThank" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>❤️ Thank you for staying with me ❤️</h1>
    <p>Seriously saying , I still remember the night , I texted u for the first time, soo nervous , scared😥, i thought u wont reply , but as soon as i texted u replyed no 🫰🫰</p>
    <button onclick="showScreen('bond')">Next</button>
  </div>
</div>

<!-- PAGE 5 -->
<div id="screenBond" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>💞 Please don’t leave me 💞</h1>
    <p>Still now ur the one listens to my stupid talks, In no friendship or realtionship , i hv seen a gurl  text first , always the boys only text, but but!!!!, , u always text me first , i become soo excited seeing ur text 🥰🥰🥰🥰, my days starts with ur gud mrng and ends with ur gud night💕💕, soo much i am addicted to u, soo plzz dont forget me or lv me😃 </p>
    <button onclick="showScreen('sorry')">Next</button>
  </div>
</div>

<!-- PAGE 6 -->
<div id="screenSorry" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>🙏 Sorry mahh 🙏</h1>
    <p>Sorry,mahh in case , or in any point of time , if i hv hurted u or made u feel bad😔😔😓😓</p>
    <button onclick="showScreen('trust')">Next</button>
  </div>
</div>

<!-- PAGE 7 (Trust) -->
<div id="screenTrust" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>🤝 The trust you have on me 🤝</h1>
    <p>Thankyou soo much for the trust u hv  on me , ig no gurl gives her insta password and all , u had trust on mee , thank u soooo much!!🫡🫡
      i am suree tht , in any point of time , I wont break ur trust💖
    </p>
    <button onclick="showScreen('heartfelt')">Next</button>
  </div>
</div>

<!-- PAGE 8 -->
<div id="screenHeartfelt" class="screen">
  <img src="heart png.png" class="shinchan">
  <div class="text-container">
    <h1>🌸 ALWAYS FIRST PRIORITY 🌸</h1>
    <p>You’re my first priority, always 💖</p>
    <button onclick="showScreen('princess')">Next</button>
  </div>
</div>

<!-- PAGE 9 (Princess) -->
<div id="screenPrincess" class="screen">
  <img src="https://github.com/kool00/finaltrial/blob/main/princess.png?raw=true" class="shinchan">
  <div class="text-container">
    <h1>👑 You’re my princess 👑</h1>
    <p>Your beauty shines brighter than anything 💖</p>
    <button onclick="showScreen('memories')">Next</button>
  </div>
</div>

<!-- PAGE 10 (Memories) -->
<div id="screenMemories" class="screen">
  <div class="text-container">
    <h1>📸 Our Memories 📸</h1>
    <img id="memImage" class="memories-img slide-active" src="mem1.jpg" alt="Memory">
    <div>
      <button onclick="prevMemory()">Previous</button>
      <button onclick="nextMemory()">Next</button>
    </div>
  </div>
</div>

<!-- PAGE 11 (Final) -->
<div id="screenFinal" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan">
  <div class="text-container">
    <h1>🎆 Happy New Year again! 🥳</h1>
    <p>May this new year bring endless joy and love 💖</p>
  </div>
</div>

<script>
let currentScreen = 1;
function showScreen(next) {
  document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
  switch(next){
    case 'like': document.getElementById('screenLike').classList.add('active'); break;
    case 'goodGirl': document.getElementById('screenGoodGirl').classList.add('active'); break;
    case 'please': document.getElementById('screenPlease').classList.add('active'); break;
    case 'thank': document.getElementById('screenThank').classList.add('active'); break;
    case 'bond': document.getElementById('screenBond').classList.add('active'); break;
    case 'sorry': document.getElementById('screenSorry').classList.add('active'); break;
    case 'trust': document.getElementById('screenTrust').classList.add('active'); break;
    case 'heartfelt': document.getElementById('screenHeartfelt').classList.add('active'); break;
    case 'princess': document.getElementById('screenPrincess').classList.add('active'); break;
    case 'memories': document.getElementById('screenMemories').classList.add('active'); break;
    case 'final': document.getElementById('screenFinal').classList.add('active'); break;
  }
}

/* Hearts floating */
function startHearts() {
  setInterval(() => {
    const heart = document.createElement('div');
    heart.classList.add('heart');
    heart.innerHTML = '❤️';
    heart.style.left = Math.random() * 100 + 'vw';
    heart.style.fontSize = Math.random() * 20 + 10 + 'px';
    heart.style.animationDuration = 4 + Math.random() * 3 + 's';
    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 7000);
  }, 400);
}
startHearts();

/* Fireworks */
const canvas = document.getElementById("fireworks");
const ctx = canvas.getContext("2d");
let W = canvas.width = window.innerWidth;
let H = canvas.height = window.innerHeight;
window.onresize = () => { W = canvas.width = window.innerWidth; H = canvas.height = window.innerHeight; };
const particles = [];
function random(min,max){return Math.random()*(max-min)+min;}
function createFirework(){
  const x=random(0,W), y=H, color=`hsl(${random(0,360)},100%,60%)`;
  for(let i=0;i<60;i++){ // doubled particles
    particles.push({x,y,r:random(1,3),dx:random(-4,4),dy:random(-10,-4),life:random(60,120),color});
  }
}
function drawFireworks(){
  ctx.clearRect(0,0,W,H);
  for(let i=0;i<particles.length;i++){
    const p=particles[i];
    ctx.beginPath();
    ctx.arc(p.x,p.y,p.r,0,2*Math.PI);
    ctx.fillStyle=p.color;
    ctx.fill();
    p.x+=p.dx; p.y+=p.dy; p.dy+=0.15; p.life--;
  }
  for(let i=particles.length-1;i>=0;i--){if(particles[i].life<=0)particles.splice(i,1);}
  requestAnimationFrame(drawFireworks);
}
setInterval(createFirework,400); // faster bursts
drawFireworks();

/* Memories slideshow */
let memIndex = 1;
const memTotal = 10;
const memImg = document.getElementById('memImage');
function showMemory(idx, dir){
  memImg.classList.remove('slide-active');
  memImg.classList.add(dir === 'next' ? 'slide-in-right' : 'slide-in-left');
  setTimeout(()=>{
    memImg.src = `mem${idx}.jpg`;
    memImg.classList.remove('slide-in-right','slide-in-left');
    memImg.classList.add('slide-active');
  },300);
}
function nextMemory(){
  if(memIndex < memTotal) { memIndex++; showMemory(memIndex, 'next'); }
  else showScreen('final');
}
function prevMemory(){
  if(memIndex > 1) { memIndex--; showMemory(memIndex, 'prev'); }
}
</script>

</body>
</html>
