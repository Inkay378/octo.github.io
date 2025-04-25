<!DOCTYPE html>
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
      color: #76ff03;
      border-bottom: 4px solid #76ff03;
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
      border-left: 6px solid #76ff03;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
    }
    h2 {
      font-family: 'Orbitron', sans-serif;
      color: #76ff03;
      margin-bottom: 15px;
    }
    a {
      color: #76ff03;
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
      border-left: 4px solid #76ff03;
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
      <h2>Contact</h2>
      <p>If you'd like to get in touch, feel free to reach out to my email: <strong>garciainaky616@gmail.com</strong></p>
    </section>
  </main>
  <footer>
    &copy; @2025 Inaky. All rights reserved.
  </footer>
</body>
</html>
