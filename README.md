# simple-frame-work

🌟 Step into My Creative Universe! Welcome to My Website! 🌟:        https://aryanchowdhury-art.github.io/simple-frame-work/


This framework simplifies chatbot development and deployment. Features include:  Modular Design: Customizable modules for data processing, model training, and evaluation. Cross-Platform: Supports various languages and platforms. Extensible: Easy to add custom components. Interactive Interface: User-friendly for development and testing.

--------------------------------------------------------------------------------- HTML ----------------------------------------------------------------------------------------------------------------------

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>oscowl projects</title>
  <link rel="stylesheet" href="index.css">
</head>
<body>
  <canvas id="canvas"></canvas>
  <nav>
    <ul>
      <li><img class="logo" src="oscowl_logo.jpg" alt="logo"></li>
    </ul>
  </nav>
  <div class="wrapper">
    <div class="typing-demo">
      <h1>This is a long title to show</h1>
    </div>
  </div>
  <section class="content">
    <article class="about-us">
      <section class="about-content">
        <h2>About Us</h2>
        <p>"Artificial intelligence based AI" is a bit redundant. AI, or Artificial Intelligence, by definition refers to intelligence demonstrated by machines, as opposed to natural intelligence displayed by humans and animals. So, all AI is inherently 'artificial intelligence based'.</p>
      </section>
    </article>
    <div class="flex-container">
      <section class="text-section">
        <h2>AI in Different Fields</h2>
        <p>AI is used in a variety of fields such as healthcare, finance, and entertainment. It powers applications ranging from virtual assistants to predictive analytics, helping to improve efficiency and enable new capabilities across industries.</p>
      </section>
      <section class="image-gallery">
        <img src="images/a.jpg" alt="Image 1">
        <img src="images/b.jpg" alt="Image 2">
        <img src="images/c.jpg" alt="Image 3">
        <img src="images/d.jpg" alt="Image 4">
        <img src="images/e.jpg" alt="Image 5">
      </section>
    </div>
  </section>
  <script src="index.js"></script>
</body>
</html>



-----------------------------------------------------------------------------------   CSS    -----------------------------------------------------------------------------------------------------------------

body {
  padding: 0;
  margin: 0;
  height: 100vh;
  overflow: hidden;
  font-family: Arial, sans-serif;
  color: #fff;
}

#canvas {
  position: fixed;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: #050303;
}

nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 10;
}

nav ul li {
  display: inline-block;
}

nav ul img {
  width: 50px;
  height: 50px;
  border-radius: 50%;
}

.wrapper {
  height: 30vh;
  display: grid;
  place-items: center;
  z-index: 5;
  position: relative;
}

.typing-demo {
  width: 44ch;
  animation: typing 2s steps(44), blink .5s step-end infinite alternate;
  white-space: nowrap;
  overflow: hidden;
  border-right: 3px solid;
  font-family: monospace;
  font-size: 2em;
  color: #fff;
}

@keyframes typing {
  from { width: 0; }
}

@keyframes blink {
  50% { border-color: transparent; }
}

.content {
  position: relative;
  z-index: 5;
  padding: 20px;
  overflow-y: auto;
  height: 50vh;
  box-sizing: border-box;
}

.about-us {
  background: linear-gradient(145deg, #444444, #222222);
  padding: 40px;
  margin: 20px auto;
  border-radius: 10px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.4);
  color: #fff;
  max-width: 800px;
  position: relative;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.about-us::before {
  content: "";
  position: absolute;
  top: 0;
  left: 50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle at center, rgba(255, 255, 255, 0.1), transparent);
  transform: translateX(-50%) translateY(-50%);
  animation: rotate 20s linear infinite;
}

@keyframes rotate {
  0% {
    transform: translateX(-50%) translateY(-50%) rotate(0deg);
  }
  100% {
    transform: translateX(-50%) translateY(-50%) rotate(360deg);
  }
}

.about-content {
  position: relative;
  z-index: 1;
  text-align: center;
}

.about-us h2 {
  font-size: 2.5em;
  margin-bottom: 20px;
  position: relative;
  display: inline-block;
  padding-bottom: 10px;
  border-bottom: 2px solid #00b4d8;
}

.about-us p {
  font-size: 1.2em;
  line-height: 1.6;
}

.about-us p::first-letter {
  font-size: 1.5em;
  font-weight: bold;
  color: #00b4d8;
  margin-right: 5px;
}

.flex-container {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin: 20px auto;
  max-width: 800px;
  width: 100%;
}

.text-section {
  background: linear-gradient(145deg, #333333, #111111);
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.4);
  color: #fff;
  width: 50%;
  box-sizing: border-box;
}

.text-section h2 {
  font-size: 2em;
  margin-bottom: 15px;
  border-bottom: 2px solid #00b4d8;
  display: inline-block;
}

.text-section p {
  font-size: 1.1em;
  line-height: 1.6;
  margin-bottom: 10px;
}

.image-gallery {
  display: grid;
  grid-template-columns: repeat(5, 100px);
  grid-template-rows: repeat(5, 100px);
  gap: 10px;
  padding: 10px;
}

.image-gallery img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
  transition: transform 0.3s ease, z-index 0.3s;
}

.image-gallery img.zoomed {
  transform: scale(1.5);
  z-index: 10;
}

/* Position the images diagonally */
.image-gallery img:nth-child(1) {
  grid-column: 1;
  grid-row: 1;
}

.image-gallery img:nth-child(2) {
  grid-column: 2;
  grid-row: 2;
}

.image-gallery img:nth-child(3) {
  grid-column: 3;
  grid-row: 3;
}

.image-gallery img:nth-child(4) {
  grid-column: 4;
  grid-row: 4;
}

.image-gallery img:nth-child(5) {
  grid-column: 5;
  grid-row: 5;
}
---------------------------------------------------------------------------------------  java script ---------------------------------------------------------------------------------------------------------


let canvas, ctx, w, h, units;
let unitCount = 100;
let hue = 0;

function init() {
  canvas = document.querySelector("#canvas");
  ctx = canvas.getContext("2d");

  resizeReset();
  createUnits();
  animationLoop();
  addScrollZoomEffect();
}

function resizeReset() {
  w = canvas.width = window.innerWidth;
  h = canvas.height = window.innerHeight;
  
  ctx.fillStyle = "#222";
  ctx.fillRect(0, 0, w, h);
}

function createUnits() {
  units = [];
  for (let i = 0; i < unitCount; i++) {
    setTimeout(() => {
      units.push(new Unit());
    }, i * 200);
  }
}

function animationLoop() {
  ctx.fillStyle = "rgba(0, 0, 0, .05)";
  ctx.fillRect(0, 0, w, h);

  drawScene();  
  requestAnimationFrame(animationLoop);
}

function drawScene() {
  for (let i = 0; i < units.length; i++) {
    units[i].update();
    units[i].draw();
  }
}

function getRandomInt(min, max) {
  return Math.round(Math.random() * (max - min)) + min;
}

class Unit {
  constructor() {
    this.reset();
    this.constructed = true;
  }
  reset() {
    this.x = Math.round(w / 2);
    this.y = Math.round(h / 2);
    this.sx = this.x;
    this.sy = this.y;
    this.angle = 60 * getRandomInt(0, 5);
    this.size = 1;
    this.radian = (Math.PI / 180) * (this.angle + 90);
    this.speed = 2;
    this.maxDistance = 30;
    this.time = 0;
    this.ttl = getRandomInt(180, 300);
    this.hue = hue;
    hue += 0.5;
  }
  draw() {
    ctx.save();
    ctx.beginPath();    
    ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
    ctx.fillStyle = `hsl(${this.hue}, 100%, 50%)`;
    ctx.shadowColor = `hsl(${this.hue}, 100%, 50%)`;
    ctx.shadowBlur = 5;
    ctx.fill();
    ctx.closePath();
    ctx.restore();
  }
  update() {
    let dx = this.sx - this.x;
    let dy = this.sy - this.y;
    let distance = Math.sqrt(dx * dx + dy * dy);

    if (distance >= this.maxDistance) {
      if (getRandomInt(0, 1)) {
        this.angle += 60;
      } else {
        this.angle -= 60;
      }

      this.radian = (Math.PI / 180) * (this.angle + 90);
      this.sx = this.x;
      this.sy = this.y; 
    }

    this.x += this.speed * Math.sin(this.radian);
    this.y += this.speed * Math.cos(this.radian);
    
    if (this.time >= this.ttl || this.x < 0 || this.x > w || this.y < 0 || this.y > h) {
      this.reset();
    }

    this.time++;
  }
}

function addScrollZoomEffect() {
  const images = document.querySelectorAll(".image-gallery img");
  let currentIndex = -1;
  const imageHeight = images[0].clientHeight;
  
  window.addEventListener("scroll", () => {
    const scrollTop = window.pageYOffset || document.documentElement.scrollTop;
    const newCurrentIndex = Math.min(images.length - 1, Math.floor(scrollTop / imageHeight));

    if (newCurrentIndex !== currentIndex) {
      if (currentIndex >= 0) {
        images[currentIndex].classList.remove("zoomed");
      }
      images[newCurrentIndex].classList.add("zoomed");
      currentIndex = newCurrentIndex;
    }
  });
}

window.addEventListener("DOMContentLoaded", init);
window.addEventListener("resize", resizeReset);
