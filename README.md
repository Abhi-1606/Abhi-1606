# Hey there! 👋 I'm Abhishek

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=28&pause=1000&color=00D9FF&center=true&width=600&lines=Web+Developer+%7C+Competitive+Programmer;Building+Beautiful+Web+Applications;Always+Learning%2C+Always+Building" alt="Typing SVG" />
</div>

---

## 🚀 About Me

I'm a **second-year B.Tech student** from **Bengaluru, India**, passionate about building intuitive and visually stunning web applications. I love solving complex problems through code and continuously improving my skills in modern web technologies.

### 💻 What I Do
- **Web Development**: Creating responsive, interactive applications with HTML, CSS, and JavaScript
- **Competitive Programming**: Solving algorithmic challenges and improving problem-solving skills
- **UI/UX Design**: Designing polished interfaces and seamless user experiences
- **Full Stack Development**: Currently learning MERN stack for end-to-end application development

---

## 🛠️ Tech Stack

### Languages
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34C26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### Tools & Platforms
![VS Code](https://img.shields.io/badge/VS%20Code-0078D4?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

---

## 🌟 Featured Projects

### 🎵 [Spotify Login Page](https://github.com/Abhi-1606/spotify-login-page)
A beautiful recreation of Spotify's login interface with modern CSS and responsive design.

### 🛒 [Amazon Clone](https://github.com/Abhi-1606/Amazon-clone)
Full-featured Amazon clone demonstrating e-commerce principles and UI implementation.

### 💼 [Portfolio](https://github.com/Abhi-1606/Portfolio)
Personal portfolio website showcasing my projects and skills with elegant animations.

### 💪 [HackerRank Solutions](https://github.com/Abhi-1606/Hacker-Rank)
Comprehensive collection of HackerRank problem solutions in multiple languages.

---

## 🎮 Interactive Snake Game

<div align="center">

### 🐍 Play Snake - Eat Countries Edition!

Click the link below to play an interactive snake game where your snake grows by eating country territories!

[![Play Snake Game](https://img.shields.io/badge/🐍%20Play%20Snake%20Game-Click%20Here-ff69b4?style=for-the-badge&logo=gamepad&logoColor=white)](https://Abhi-1606.github.io/snake-game/)

**Features:**
- 🌍 Eat virtual country territories to grow
- 📈 Progressive difficulty as you score
- 🎯 Real-time score tracking
- ⌨️ Smooth keyboard controls (Arrow Keys)
- 📱 Mobile-friendly responsive design



---

## 📊 GitHub Stats


---

## 🎯 Currently

- 🔧 Building full-stack web applications with **MERN Stack**
- 📚 Preparing for **competitive programming** challenges
- 🎨 Improving **UI/UX design** and animation skills
- 📖 Learning advanced **JavaScript** concepts
- 🐍 Creating interactive games and web experiences

---

## 🤝 Let's Connect!

<div align="center">
  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Abhi-1606)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:your.email@example.com)

</div>

---

## 📝 Fun Facts

- 🎬 Loves anime, especially isekai and fantasy genres
- 🏎️ Follows F1 racing and cricket (India vs New Zealand enthusiast!)
- 💡 Believes in writing clean, readable code
- ⚡ Quick learner who enjoys solving real-world problems

---

---

## 🐍 My Contributions

<div align="center">

### Interactive Snake Game - Eat My Contributions!

Watch the snake navigate through my contribution graph! Click the canvas or use arrow keys to play.

<canvas id="snakeGameCanvas" width="600" height="200" style="border: 3px solid #00D9FF; background-color: #0d1117; cursor: pointer; display: block; margin: 20px auto;"></canvas>

**Controls:** Arrow Keys or Mouse Clicks (tap different areas to change direction)

<script>
  const canvas = document.getElementById('snakeGameCanvas');
  if (canvas) {
    const ctx = canvas.getContext('2d');
    const gridSize = 20;
    const cols = canvas.width / gridSize;
    const rows = canvas.height / gridSize;
    
    let snake = [{x: 10, y: 10}];
    let food = {x: Math.floor(Math.random() * cols), y: Math.floor(Math.random() * rows)};
    let dx = 1;
    let dy = 0;
    let nextDx = 1;
    let nextDy = 0;
    let score = 0;
    let gameRunning = true;
    
    function drawGame() {
      // Clear canvas
      ctx.fillStyle = '#0d1117';
      ctx.fillRect(0, 0, canvas.width, canvas.height);
      
      // Draw grid
      ctx.strokeStyle = '#1f2937';
      ctx.lineWidth = 0.5;
      for (let i = 0; i <= cols; i++) {
        ctx.beginPath();
        ctx.moveTo(i * gridSize, 0);
        ctx.lineTo(i * gridSize, canvas.height);
        ctx.stroke();
      }
      for (let i = 0; i <= rows; i++) {
        ctx.beginPath();
        ctx.moveTo(0, i * gridSize);
        ctx.lineTo(canvas.width, i * gridSize);
        ctx.stroke();
      }
      
      // Draw food (green - contribution color)
      ctx.fillStyle = '#1f6934';
      ctx.fillRect(food.x * gridSize + 2, food.y * gridSize + 2, gridSize - 4, gridSize - 4);
      
      // Draw snake
      for (let i = 0; i < snake.length; i++) {
        if (i === 0) {
          ctx.fillStyle = '#00D9FF'; // Head - cyan
        } else {
          ctx.fillStyle = '#0891b2'; // Body - darker cyan
        }
        ctx.fillRect(snake[i].x * gridSize + 2, snake[i].y * gridSize + 2, gridSize - 4, gridSize - 4);
      }
      
      // Draw score
      ctx.fillStyle = '#00D9FF';
      ctx.font = 'bold 16px Arial';
      ctx.fillText('Score: ' + score, 10, 25);
    }
    
    function update() {
      dx = nextDx;
      dy = nextDy;
      
      let head = {x: snake[0].x + dx, y: snake[0].y + dy};
      
      // Wrap around
      head.x = (head.x + cols) % cols;
      head.y = (head.y + rows) % rows;
      
      // Check collision with self
      for (let i = 0; i < snake.length; i++) {
        if (head.x === snake[i].x && head.y === snake[i].y) {
          gameRunning = false;
          return;
        }
      }
      
      snake.unshift(head);
      
      // Check if ate food
      if (head.x === food.x && head.y === food.y) {
        score++;
        food = {x: Math.floor(Math.random() * cols), y: Math.floor(Math.random() * rows)};
      } else {
        snake.pop();
      }
    }
    
    function gameLoop() {
      if (gameRunning) {
        update();
        drawGame();
        setTimeout(gameLoop, 100);
      } else {
        // Game over
        ctx.fillStyle = 'rgba(0, 0, 0, 0.5)';
        ctx.fillRect(0, 0, canvas.width, canvas.height);
        ctx.fillStyle = '#FF6B6B';
        ctx.font = 'bold 32px Arial';
        ctx.textAlign = 'center';
        ctx.fillText('Game Over!', canvas.width / 2, canvas.height / 2 - 20);
        ctx.font = '20px Arial';
        ctx.fillText('Final Score: ' + score, canvas.width / 2, canvas.height / 2 + 20);
      }
    }
    
    // Keyboard controls
    document.addEventListener('keydown', function(e) {
      if (e.key === 'ArrowUp' && dy === 0) { nextDx = 0; nextDy = -1; e.preventDefault(); }
      if (e.key === 'ArrowDown' && dy === 0) { nextDx = 0; nextDy = 1; e.preventDefault(); }
      if (e.key === 'ArrowLeft' && dx === 0) { nextDx = -1; nextDy = 0; e.preventDefault(); }
      if (e.key === 'ArrowRight' && dx === 0) { nextDx = 1; nextDy = 0; e.preventDefault(); }
    });
    
    // Mouse controls
    canvas.addEventListener('click', function(e) {
      const rect = canvas.getBoundingClientRect();
      const x = e.clientX - rect.left;
      const y = e.clientY - rect.top;
      const centerX = rect.width / 2;
      const centerY = rect.height / 2;
      
      if (x < centerX - 30 && Math.abs(y - centerY) < 30 && dx === 0) {
        nextDx = -1; nextDy = 0;
      } else if (x > centerX + 30 && Math.abs(y - centerY) < 30 && dx === 0) {
        nextDx = 1; nextDy = 0;
      } else if (y < centerY - 30 && Math.abs(x - centerX) < 30 && dy === 0) {
        nextDx = 0; nextDy = -1;
      } else if (y > centerY + 30 && Math.abs(x - centerX) < 30 && dy === 0) {
        nextDx = 0; nextDy = 1;
      }
    });
    
    // Start game
    gameLoop();
  }
</script>

**How to Play:**
- 🐍 Use Arrow Keys or Click to move the snake
- 🟢 Eat the green contribution squares to grow
- ⚠️ Don't hit yourself!
- 🔄 Game wraps around edges

This snake game represents my coding journey - constantly growing, always contributing!

</div>

<div align="center">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=dark" />
</div>

<div align="center">
  <sub>✨ Feel free to reach out for collaborations or just a friendly chat! ✨</sub>
</div>
