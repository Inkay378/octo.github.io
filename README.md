<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Inaky Hub</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: radial-gradient(circle at center, #0f172a, #060d1f);
      color: #dbeafe;
      text-align: center;
    }
    header {
      padding: 30px 20px;
    }
    header h1 {
      font-size: 3em;
      color: #a78bfa;
      text-shadow: 0 0 12px #a78bfa;
    }
    nav {
      margin: 30px 0;
    }
    nav a {
      background: transparent;
      border: 2px solid #a78bfa;
      padding: 10px 20px;
      margin: 0 10px;
      color: #dbeafe;
      border-radius: 10px;
      text-decoration: none;
      font-weight: bold;
      transition: all 0.3s ease;
      box-shadow: 0 0 10px #a78bfa;
    }
    nav a:hover {
      background-color: #a78bfa;
      color: #0f172a;
    }
    .section {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
    }
    .script-box {
      text-align: left;
      background: #1e293b;
      padding: 20px;
      border-radius: 10px;
      margin: 20px 0;
      color: #f1f5f9;
      white-space: pre-wrap;
      word-wrap: break-word;
      box-shadow: 0 0 15px #a78bfa;
    }
    .video {
      margin-top: 20px;
      box-shadow: 0 0 25px #a78bfa;
      border-radius: 12px;
    }
    footer {
      margin-top: 50px;
      padding: 20px;
      background: #0e1a2b;
      color: #64748b;
      font-size: 0.9em;
    }
  </style>
</head>
<body>
  <header>
    <h1>Inaky Hub</h1>
    <p>Scripts, Tools, and Good Vibes Only</p>
  </header>

  <nav>
    <a href="#scripts">Scripts</a>
    <a href="#video">Video</a>
    <a href="#contact">Contact</a>
  </nav>

  <section class="section" id="scripts">
    <h2>🔥 Game Scripts</h2>

    <div class="script-box">
      <strong>TSB Launcher:</strong><br>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/10tempest01/tempest-hub/refs/heads/main/Launcher.lua"))()
    </div>

    <div class="script-box">
      <strong>MADARA Moveset:</strong><br>
      getgenv().Cutscene = True<br>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/LolnotaKid/SCRIPTSBYVEUX/refs/heads/main/BoombasticLol.lua.txt"))()
    </div>

    <div class="script-box">
      <strong>Minos Prime Fix:</strong><br>
      _G.SkipIntro = true<br>
      _G.Night = false<br>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/S1gmaGuy/MinosPrimeFixed/refs/heads/main/ThefixIsSoSigma"))()
    </div>

    <div class="script-box">
      <strong>Very OP Hub:</strong><br>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/ATrainz/Phantasm/refs/heads/main/Games/TSB.lua"))()
    </div>

    <div class="script-box">
      <strong>Tamhub:</strong><br>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/tamarixr/tamhub/main/bettertamhub.lua"))()
    </div>

    <div class="script-box">
      <strong>Infinite Yield:</strong><br>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
    </div>

    <div class="script-box">
      <strong>UNC Test:</strong><br>
      loadstring(game:HttpGet('https://github.com/ltseverydayyou/uuuuuuu/blob/main/UNC%20test?raw=true'))()
    </div>
  </section>

  <section class="section" id="video">
    <h2>🎥 KJ & Friends</h2>
    <iframe class="video" width="560" height="315" src="https://www.youtube.com/embed/MCy7yx3fSTY" frameborder="0" allowfullscreen></iframe>
  </section>

  <section class="section" id="contact">
    <h2>📫 Contact</h2>
    <p>Hit me up at <strong>garciainaky616@gmail.com</strong> if you need help or got cool scripts 😎</p>
  </section>

  <footer>
    Made by Inaky's chat gpt prompts
  </footer>
</body>
</html>
