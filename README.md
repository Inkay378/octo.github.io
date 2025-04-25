<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Inaky Hub</title>
  <link rel="icon" href="https://guns.lol/favicon.ico" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #121212;
      color: #e0e0e0;
      overflow-x: hidden;
      text-align: center;
    }

    h1, h2 {
      color: #a78bfa;
      text-shadow: 0 0 10px #a78bfa;
    }

    nav {
      background: #1a1a1a;
      padding: 1rem 0;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .nav-center {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
    }

    .nav-center a {
      color: #e0e0e0;
      text-decoration: none;
      padding: 10px 15px;
      font-weight: bold;
      border-radius: 8px;
      transition: all 0.3s ease;
      cursor: pointer;
    }

    .nav-center a:hover,
    .nav-center a.active {
      color: #a78bfa;
      background-color: rgba(167, 139, 250, 0.1);
    }

    .section {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
      animation: fadeInUp 0.6s ease;
      display: none;
    }

    .section.active {
      display: block;
    }

    .script-box {
      text-align: left;
      background: #1e1e1e;
      padding: 20px;
      border-radius: 10px;
      margin: 20px 0;
      color: #f1f5f9;
      white-space: pre-wrap;
      word-wrap: break-word;
      box-shadow: 0 0 15px #a78bfa;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
      padding: 40px 20px;
      max-width: 1200px;
      margin: auto;
    }

    .feature-card {
      background: #1a1a1a;
      border-radius: 12px;
      padding: 30px 20px;
      text-align: center;
      color: #e0e0e0;
      box-shadow: 0 0 12px rgba(255, 255, 255, 0.05);
      transition: all 0.3s ease;
      border: 1px solid transparent;
    }

    .feature-card:hover {
      border: 1px solid white;
      background: #1f1f1f;
      box-shadow: 0 0 15px white;
    }

    .feature-card i {
      display: inline-block;
      font-size: 1.8rem;
      margin-bottom: 15px;
      color: #a78bfa;
    }

    .feature-card h3 {
      margin-bottom: 10px;
      font-size: 1.2rem;
      font-weight: bold;
      color: white;
    }

    .feature-card p {
      font-size: 0.95rem;
      color: #cbd5e1;
    }

    .video {
      margin-top: 20px;
      box-shadow: 0 0 25px #a78bfa;
      border-radius: 12px;
    }

    .btn-discord {
      display: inline-block;
      margin-top: 20px;
      background-color: #a78bfa;
      color: #0f172a;
      padding: 12px 24px;
      border-radius: 10px;
      font-weight: bold;
      text-decoration: none;
      font-size: 1.1rem;
      box-shadow: 0 0 20px #a78bfa;
      transition: background 0.3s, transform 0.3s;
    }

    .btn-discord:hover {
      background-color: #c4b5fd;
      transform: scale(1.05);
    }

    footer {
      margin-top: 50px;
      padding: 20px;
      background: #1a1a1a;
      color: #64748b;
      font-size: 0.9em;
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
</head>
<body>

  <header class="section active">
    <h1>Inaky Hub</h1>
    <p>Scripts, Tools, and Good Vibes Only</p>
  </header>

  <nav>
    <div class="nav-center">
      <a class="tab-link active" data-tab="scripts">Scripts</a>
      <a class="tab-link" data-tab="video">Video</a>
      <a class="tab-link" data-tab="discord">Discord</a>
      <a class="tab-link" data-tab="contact">Contact</a>
    </div>
  </nav>

  <section class="section active" id="scripts">
    <h2>🔥 Game Scripts</h2>
    <div class="script-box"><strong>TSB Launcher:</strong><br>loadstring(game:HttpGet("https://raw.githubusercontent.com/10tempest01/tempest-hub/refs/heads/main/Launcher.lua"))()</div>
    <div class="script-box"><strong>MADARA Moveset:</strong><br>getgenv().Cutscene = True<br>loadstring(game:HttpGet("https://raw.githubusercontent.com/LolnotaKid/SCRIPTSBYVEUX/refs/heads/main/BoombasticLol.lua.txt"))()</div>
    <div class="script-box"><strong>Minos Prime Fix:</strong><br>_G.SkipIntro = true<br>_G.Night = false<br>loadstring(game:HttpGet("https://raw.githubusercontent.com/S1gmaGuy/MinosPrimeFixed/refs/heads/main/ThefixIsSoSigma"))()</div>
    <div class="script-box"><strong>Very OP Hub:</strong><br>loadstring(game:HttpGet("https://raw.githubusercontent.com/ATrainz/Phantasm/refs/heads/main/Games/TSB.lua"))()</div>
    <div class="script-box"><strong>Tamhub:</strong><br>loadstring(game:HttpGet("https://raw.githubusercontent.com/tamarixr/tamhub/main/bettertamhub.lua"))()</div>
    <div class="script-box"><strong>Infinite Yield:</strong><br>loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()</div>
    <div class="script-box"><strong>UNC Test:</strong><br>loadstring(game:HttpGet('https://github.com/ltseverydayyou/uuuuuuu/blob/main/UNC%20test?raw=true'))()</div>
  </section>

  <section class="section" id="video">
    <h2>🎥watch if ur bored</h2>
  <div class="video-grid">
  <iframe class="video" src="https://www.youtube.com/embed/MCy7yx3fSTY" frameborder="0" allowfullscreen></iframe>
  <iframe class="video" src="https://www.youtube.com/embed/VIDEO_ID_2" frameborder="0" allowfullscreen></iframe>
  <iframe class="video" src="https://www.youtube.com/embed/VIDEO_ID_3" frameborder="0" allowfullscreen></iframe>
</div>
  </section>

  <section class="section" id="discord">
    <h2>💬 Join My Discord</h2>
    <p>Come hang out, get updates, share scripts, or just vibe with the squad.</p>
    <a href="https://discord.gg/EyseXZMm" target="_blank" class="btn-discord">Join the Discord</a>
  </section>

  <section class="section" id="contact">
    <h2>📫 Contact</h2>
    <p>Hit me up at <strong>garciainaky616@gmail.com</strong> if you need help or got cool scripts 😎</p>
  </section>

  <footer>
    Made by Inaky's chat gpt prompts
  </footer>

  <script>
    const tabLinks = document.querySelectorAll(".tab-link");
    const sections = document.querySelectorAll(".section");

    tabLinks.forEach(link => {
      link.addEventListener("click", () => {
        // Remove active from all
        tabLinks.forEach(l => l.classList.remove("active"));
        sections.forEach(s => s.classList.remove("active"));

        // Add active to clicked
        link.classList.add("active");
        document.getElementById(link.getAttribute("data-tab")).classList.add("active");
      });
    });
  </script>

</body>
</html>
