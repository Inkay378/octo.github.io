<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Welcome to Inaky's Website</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Roboto&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Roboto', sans-serif;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: #eee;
      line-height: 1.6;
    }
    header {
      background: #1e1e2f;
      padding: 40px 20px;
      text-align: center;
      color: #d9a7ff;
      border-bottom: 4px solid #d9a7ff;
    }
    header h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: 3rem;
      margin-bottom: 10px;
    }
    main {
      padding: 30px;
      max-width: 1100px;
      margin: auto;
    }
    section {
      background: #1e1e2f;
      padding: 25px;
      margin-bottom: 30px;
      border-left: 6px solid #d9a7ff;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
    }
    h2 {
      font-family: 'Orbitron', sans-serif;
      color: #d9a7ff;
      margin-bottom: 15px;
    }
    a {
      color: #d9a7ff;
      text-decoration: none;
    }
    .scripts-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 15px;
    }
    .script-block {
      background-color: #2c2c2c;
      padding: 15px;
      border-left: 4px solid #d9a7ff;
      border-radius: 5px;
      font-family: 'Courier New', Courier, monospace;
      color: #f1f1f1;
      white-space: pre-wrap;
      word-wrap: break-word;
    }
    iframe {
      width: 100%;
      height: 315px;
      border: none;
      border-radius: 8px;
    }
    canvas {
      background-color: #111;
      display: block;
      margin: 0 auto;
      border: 2px solid #d9a7ff;
    }
    footer {
      background-color: #111;
      color: #aaa;
      text-align: center;
      padding: 15px;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to Inaky's Website</h1>
    <p>Building something amazing with code</p>
  </header>
  <main>
    <section>
      <h2>About Me</h2>
      <p>Hi! I'm Inaky, and here are some scripts for u bum.</p>
    </section>

    <section>
      <h2>Game Scripts</h2>
      <div class="scripts-container">
        <div class="script-block">
          <strong>Tsb:</strong>
          loadstring(game:HttpGet("https://raw.githubusercontent.com/10tempest01/tempest-hub/refs/heads/main/Launcher.lua"))()
        </div>
        <div class="script-block">
          <strong>MADARA Moveset:</strong>
          getgenv().Cutscene = True
          loadstring(game:HttpGet("https://raw.githubusercontent.com/LolnotaKid/SCRIPTSBYVEUX/refs/heads/main/BoombasticLol.lua.txt"))()
        </div>
        <div class="script-block">
          <strong>Minos Prime:</strong>
          _G.SkipIntro = true
          _G.Night = false
          loadstring(game:HttpGet("https://raw.githubusercontent.com/S1gmaGuy/MinosPrimeFixed/refs/heads/main/ThefixIsSoSigma"))()
        </div>
        <div class="script-block">
          <strong>Very OP Hub:</strong>
          loadstring(game:HttpGet("https://raw.githubusercontent.com/ATrainz/Phantasm/refs/heads/main/Games/TSB.lua"))()
        </div>
        <div class="script-block">
          <strong>Infinite Yield:</strong>
          loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
        </div>
        <div class="script-block">
          <strong>Unc Test:</strong>
          loadstring(game:HttpGet('https://github.com/ltseverydayyou/uuuuuuu/blob/main/UNC%20test?raw=true'))()
        </div>
      </div>
    </section>

    <section>
      <h2>Featured Video</h2>
      <iframe src="https://www.youtube.com/embed/MCy7yx3fSTY" allowfullscreen></iframe>
    </section>

    <section>
      <h2>Snake Game</h2>
      <canvas id="game" width="400" height="400"></canvas>
      <script>
        const canvas = document.getElementById("game");
        const ctx = canvas.getContext("2d");

        const grid = 20;
        let count = 0;
        let snake = { x: 160, y: 160, dx: grid, dy: 0, cells: [], maxCells: 4 };
        let apple = { x: 320, y: 320 };

        function getRandomInt(min, max) {
          return Math.floor(Math.random() * (max - min)) + min;
        }

        function loop() {
          requestAnimationFrame(loop);

          if (++count < 4) return;
          count = 0;

          ctx.clearRect(0, 0, canvas.width, canvas.height);

          snake.x += snake.dx;
          snake.y += snake.dy;

          if (snake.x < 0) snake.x = canvas.width - grid;
          else if (snake.x >= canvas.width) snake.x = 0;
          if (snake.y < 0) snake.y = canvas.height - grid;
          else if (snake.y >= canvas.height) snake.y = 0;

          snake.cells.unshift({ x: snake.x, y: snake.y });
          if (snake.cells.length > snake.maxCells) snake.cells.pop();

          ctx.fillStyle = "#d9a7ff";
          ctx.fillRect(apple.x, apple.y, grid - 1, grid - 1);

          ctx.fillStyle = "#fff";
          snake.cells.forEach((cell, index) => {
            ctx.fillRect(cell.x, cell.y, grid - 1, grid - 1);

            if (cell.x === apple.x && cell.y === apple.y) {
              snake.maxCells++;
              apple.x = getRandomInt(0, 20) * grid;
              apple.y = getRandomInt(0, 20) * grid;
            }

            for (let i = index + 1; i < snake.cells.length; i++) {
              if (cell.x === snake.cells[i].x && cell.y === snake.cells[i].y) {
                snake.x = 160;
                snake.y = 160;
                snake.cells = [];
                snake.maxCells = 4;
                snake.dx = grid;
                snake.dy = 0;
                apple.x = getRandomInt(0, 20) * grid;
                apple.y = getRandomInt(0, 20) * grid;
              }
            }
          });
        }

        document.addEventListener("keydown", (e) => {
          if (e.key === "ArrowLeft" && snake.dx === 0) {
            snake.dx = -grid;
            snake.dy = 0;
          } else if (e.key === "ArrowUp" && snake.dy === 0) {
            snake.dy = -grid;
            snake.dx = 0;
          } else if (e.key === "ArrowRight" && snake.dx === 0) {
            snake.dx = grid;
            snake.dy = 0;
          } else if (e.key === "ArrowDown" && snake.dy === 0) {
            snake.dy = grid;
            snake.dx = 0;
          }
        });

        requestAnimationFrame(loop);
      </script>
    </section>

    <section>
      <h2>Contact</h2>
      <p>If you'd like to get in touch, feel free to reach out to my email: <strong>garciainaky616@gmail.com</strong></p>
    </section>
  </main>
  <footer>
    &copy; 2025 Inaky. All rights reserved.
  </footer>
</body>
</html>
