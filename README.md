<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Inaky Hub</title>
  <link rel="icon" href="https://guns.lol/favicon.ico" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
  <style>
    :root {
      /* Dark theme variables (default) */
      --bg-primary: #121212;
      --bg-secondary: #1a1a1a;
      --bg-tertiary: #1e1e1e;
      --text-primary: #e0e0e0;
      --text-secondary: #cbd5e1;
      --accent-color: #a78bfa;
      --accent-hover: #c4b5fd;
      --box-shadow-color: rgba(167, 139, 250, 0.5);
      --card-border: transparent;
    }

    [data-theme="light"] {
      /* Light theme variables */
      --bg-primary: #f8f9fa;
      --bg-secondary: #e9ecef;
      --bg-tertiary: #dee2e6;
      --text-primary: #212529;
      --text-secondary: #495057;
      --accent-color: #7c3aed;
      --accent-hover: #6d28d9;
      --box-shadow-color: rgba(124, 58, 237, 0.3);
      --card-border: #cbd5e1;
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: var(--bg-primary);
      color: var(--text-primary);
      overflow-x: hidden;
      text-align: center;
      transition: background-color 0.3s ease, color 0.3s ease;
    }

    h1, h2 {
      color: var(--accent-color);
      text-shadow: 0 0 10px var(--box-shadow-color);
    }

    nav {
      background: var(--bg-secondary);
      padding: 1rem 0;
      position: sticky;
      top: 0;
      z-index: 1000;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .nav-center {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
    }

    .nav-center a {
      color: var(--text-primary);
      text-decoration: none;
      padding: 10px 15px;
      font-weight: bold;
      border-radius: 8px;
      transition: all 0.3s ease;
      cursor: pointer;
    }

    .nav-center a:hover,
    .nav-center a.active {
      color: var(--accent-color);
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
      background: var(--bg-tertiary);
      padding: 20px;
      border-radius: 10px;
      margin: 20px 0;
      color: var(--text-primary);
      white-space: pre-wrap;
      word-wrap: break-word;
      box-shadow: 0 0 15px var(--box-shadow-color);
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
      background: var(--bg-secondary);
      border-radius: 12px;
      padding: 30px 20px;
      text-align: center;
      color: var(--text-primary);
      box-shadow: 0 0 12px var(--box-shadow-color);
      transition: all 0.3s ease;
      border: 1px solid var(--card-border);
    }

    .feature-card:hover {
      border: 1px solid var(--text-primary);
      background: var(--bg-tertiary);
      box-shadow: 0 0 15px var(--box-shadow-color);
    }

    .feature-card i {
      display: inline-block;
      font-size: 1.8rem;
      margin-bottom: 15px;
      color: var(--accent-color);
    }

    .feature-card h3 {
      margin-bottom: 10px;
      font-size: 1.2rem;
      font-weight: bold;
      color: var(--text-primary);
    }

    .feature-card p {
      font-size: 0.95rem;
      color: var(--text-secondary);
    }

    .video {
      margin-top: 20px;
      box-shadow: 0 0 25px var(--box-shadow-color);
      border-radius: 12px;
      width: 100%;
      max-width: 600px;
      height: 315px;
    }

    .btn-primary {
      display: inline-block;
      margin-top: 20px;
      background-color: var(--accent-color);
      color: var(--bg-primary);
      padding: 12px 24px;
      border-radius: 10px;
      font-weight: bold;
      text-decoration: none;
      font-size: 1.1rem;
      box-shadow: 0 0 20px var(--box-shadow-color);
      transition: background 0.3s, transform 0.3s;
    }

    .btn-primary:hover {
      background-color: var(--accent-hover);
      transform: scale(1.05);
    }

    footer {
      margin-top: 50px;
      padding: 20px;
      background: var(--bg-secondary);
      color: var(--text-secondary);
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
    
    /* Theme toggle styles */
    .theme-toggle {
      position: absolute;
      right: 20px;
      display: flex;
      align-items: center;
      cursor: pointer;
    }
    
    .theme-toggle-icon {
      font-size: 20px;
      margin-right: 5px;
    }
    
    .theme-toggle-text {
      font-size: 14px;
      font-weight: bold;
      color: var(--text-primary);
    }
    
    @media (max-width: 768px) {
      .theme-toggle-text {
        display: none;
      }
      
      .theme-toggle {
        right: 10px;
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
      <a class="tab-link" data-tab="scriptblox">ScriptBlox</a>
      <a class="tab-link" data-tab="discord">Discord</a>
      <a class="tab-link" data-tab="contact">Contact</a>
    </div>
    <div class="theme-toggle" id="theme-toggle">
      <span class="theme-toggle-icon">🌙</span>
      <span class="theme-toggle-text">Light Mode</span>
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
    <h2>🎥 watch if bored</h2>
    <iframe class="video" src="https://www.youtube.com/embed/LZkl0_9xFOU" frameborder="0" allowfullscreen></iframe>
    <iframe class="video" src="https://www.youtube.com/embed/hr-pUCuYALw" frameborder="0" allowfullscreen></iframe>
    <iframe class="video" src="https://www.youtube.com/embed/kMScaanmWHA" frameborder="0" allowfullscreen></iframe>
    <iframe class="video" src="https://www.youtube.com/embed/YZdl-uMfE0Y" frameborder="0" allowfullscreen></iframe>
  </section>

  <section class="section" id="scriptblox">
    <h2>📦 ScriptBlox</h2>
    <p>Discover tons of scripts directly from the official site.</p>
    <a href="https://scriptblox.com/" target="_blank" rel="noopener noreferrer" class="btn-primary">Visit ScriptBlox</a>
  </section>

  <section class="section" id="discord">
    <h2>💬 Join My Discord</h2>
    <p>Come hang out, get updates, share scripts, or just vibe with the squad.</p>
    <a href="https://discord.gg/EyseXZMm" target="_blank" rel="noopener noreferrer" class="btn-primary">Join the Discord</a>
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
    const themeToggle = document.getElementById("theme-toggle");
    const themeToggleIcon = themeToggle.querySelector(".theme-toggle-icon");
    const themeToggleText = themeToggle.querySelector(".theme-toggle-text");
    
    // Check for saved theme preference or use default
    const savedTheme = localStorage.getItem("theme") || "dark";
    document.documentElement.setAttribute("data-theme", savedTheme);
    updateThemeToggle(savedTheme);

    // Handle tab switching
    tabLinks.forEach(link => {
      link.addEventListener("click", () => {
        tabLinks.forEach(l => l.classList.remove("active"));
        sections.forEach(s => s.classList.remove("active"));

        link.classList.add("active");
        document.getElementById(link.getAttribute("data-tab")).classList.add("active");
      });
    });
    
    // Handle theme toggling
    themeToggle.addEventListener("click", () => {
      const currentTheme = document.documentElement.getAttribute("data-theme");
      const newTheme = currentTheme === "dark" ? "light" : "dark";
      
      document.documentElement.setAttribute("data-theme", newTheme);
      localStorage.setItem("theme", newTheme);
      
      updateThemeToggle(newTheme);
    });
    
    function updateThemeToggle(theme) {
      if (theme === "dark") {
        themeToggleIcon.textContent = "🌙";
        themeToggleText.textContent = "Light Mode";
      } else {
        themeToggleIcon.textContent = "☀️";
        themeToggleText.textContent = "Dark Mode";
      }
    }
  </script>

</body>
</html>
