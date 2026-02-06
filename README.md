<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AP Company — Enter the Void</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600;700&display=swap');

    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background: #000;
      color: #fff;
      overflow-x: hidden;
    }

    /* Intro Hero */
    #intro {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      position: relative;
    }

    .void-fog {
      position: absolute;
      width: 150%;
      height: 150%;
      background: radial-gradient(circle, rgba(80,0,120,0.25), rgba(0,0,0,0.9) 70%);
      filter: blur(80px);
      animation: fogmove 12s infinite ease-in-out;
    }

    @keyframes fogmove {
      0% { transform: translate(-5%, -5%) scale(1); }
      50% { transform: translate(5%, 10%) scale(1.05); }
      100% { transform: translate(-5%, -5%) scale(1); }
    }

    .hero-title {
      font-size: 4.2rem;
      letter-spacing: 8px;
      color: white;
      text-shadow: 0 0 25px rgba(140,0,255,0.8);
      z-index: 2;
    }

    #enter-btn {
      margin-top: 30px;
      padding: 15px 40px;
      font-size: 1rem;
      color: #fff;
      background: rgba(140,0,255,0.7);
      border: none;
      border-radius: 8px;
      cursor: pointer;
      text-transform: uppercase;
      letter-spacing: 2px;
      z-index: 2;
      transition: all 0.3s;
    }

    #enter-btn:hover {
      background: rgba(140,0,255,1);
      box-shadow: 0 0 20px rgba(140,0,255,0.8);
    }

    /* Main Page */
    #main {
      opacity: 0;
      pointer-events: none;
      transition: opacity 2s ease;
      padding: 150px 50px 100px;
    }

    header {
      display: flex;
      justify-content: flex-start;
      align-items: center;
      padding: 20px 50px;
      background: #050005;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 10;
      box-shadow: 0 0 20px rgba(0,0,0,0.5);
    }

    header h1 {
      font-size: 1.8rem;
      color: #fff;
      letter-spacing: 3px;
      margin-right: 50px;
    }

    nav a {
      color: #ccc;
      margin-right: 25px;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #8c00ff;
    }

    /* About Section */
    #about {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      max-width: 1000px;
      margin: 0 auto;
    }

    .section-title {
      font-size: 3rem;
      color: #8c00ff;
      margin-bottom: 30px;
      text-shadow: 0 0 15px rgba(140,0,255,0.8);
    }

    #about p {
      font-size: 1.2rem;
      line-height: 1.6;
      max-width: 800px;
      opacity: 0;
      transform: translateY(20px);
      transition: all 1s ease;
    }

    /* Subs Section */
    .subs-section {
      margin-top: 80px;
      width: 100%;
    }

    .subs-container {
      margin-top: 30px;
      display: flex;
      flex-direction: column;
      gap: 20px;
      max-width: 800px;
    }

    .sub-item {
      font-size: 1.6rem;
      color: #fff;
      background: #111;
      border: 2px solid #8c00ff;
      padding: 20px;
      border-radius: 12px;
      opacity: 0;
      transform: translateY(20px);
      transition: all 0.3s ease;
    }

    .sub-item span {
      display: block;
      font-size: 1rem;
      color: #aaa;
      margin-top: 5px;
    }

    .sub-item:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 20px rgba(140,0,255,0.5);
      cursor: pointer;
    }

    /* Contact Section */
    .contact-info {
      margin-top: 40px;
      display: flex;
      flex-direction: column;
      gap: 15px;
      max-width: 400px;
    }

    .sub-item.contact {
      font-size: 1.2rem;
      background: #111;
      border: 2px solid #8c00ff;
      padding: 15px;
      border-radius: 10px;
    }

    /* Footer */
    footer {
      margin-top: 60px;
      text-align: center;
      font-size: 1rem;
      color: #aaa;
      padding: 20px 0;
      border-top: 1px solid #8c00ff;
    }
  </style>
</head>
<body>

  <!-- Intro Section -->
  <section id="intro">
    <div class="void-fog"></div>
    <h1 class="hero-title">AP COMPANY</h1>
    <button id="enter-btn">ENTER</button>
  </section>

  <!-- Main Section -->
  <div id="main">
    <header>
      <h1>AP Company</h1>
      <nav>
        <a href="Game.html">Game</a>
        <a href="team.html">Team</a>
        <a href="#about">About</a>
      </nav>
    </header>

    <!-- About Section -->
    <section id="about">
      <h2 class="section-title">درباره ما</h2>
      <p>
        AP Company یک استودیو بازی‌سازی تاریک و مرموز است که با هدف خلق جهان‌هایی عمیق، سینمایی و داستان‌محور تأسیس شده است. 
        ما باور داریم بازی‌ها تنها سرگرمی نیستند؛ آن‌ها دروازه‌هایی به جهان‌هایی ناشناخته‌اند، جایی که هر انتخاب، هر داستان و هر تجربه بر قلب بازیکن تأثیر می‌گذارد.
      </p>

      <div class="subs-section">
        <h2 class="section-title">زیرمجموعه‌ها</h2>
        <div class="subs-container">
          <div class="sub-item">AP Craft<span>The Minecraft Server In Iran</span></div>
          <div class="sub-item">Sigma Shop<span>The Shop Is MineCraft</span></div>
        </div>

        <div class="contact-info">
          <div class="sub-item contact">@AP_Company_Official<span>ID روبیکا</span></div>
          <div class="sub-item contact">@MerVist_MC<span>پشتیبانی</span></div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer>
      AP Company By MerVist
    </footer>

  </div>

  <!-- JS -->
  <script>
    const enterBtn = document.getElementById('enter-btn');
    const intro = document.getElementById('intro');
    const main = document.getElementById('main');
    const fadeItems = document.querySelectorAll('#about p, .sub-item');

    enterBtn.addEventListener('click', () => {
      intro.style.transition = 'opacity 2s ease';
      intro.style.opacity = 0;
      setTimeout(() => {
        intro.style.display = 'none';
        main.style.opacity = 1;
        main.style.pointerEvents = 'auto';
        fadeItems.forEach((el, i) => {
          setTimeout(() => {
            el.style.opacity = 1;
            el.style.transform = 'translateY(0)';
          }, i * 600);
        });
      }, 2000);
    });
  </script>

  </body>
</html>

</body>
