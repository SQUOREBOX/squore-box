<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Squore Box – A Winner a Day</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    body {
      margin: 0;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: #0f1115;
      color: #f5f5f5;
    }
    header {
      padding: 20px 24px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      border-bottom: 1px solid #252732;
    }
    .logo {
      font-weight: 800;
      letter-spacing: 1px;
      font-size: 20px;
    }
    .tag {
      font-size: 12px;
      color: #ff8a00;
      text-transform: uppercase;
    }
    main {
      max-width: 960px;
      margin: 0 auto;
      padding: 32px 16px 64px;
    }
    .hero {
      display: grid;
      grid-template-columns: minmax(0, 2fr) minmax(0, 1.5fr);
      gap: 32px;
      align-items: center;
    }
    @media (max-width: 800px) {
      .hero {
        grid-template-columns: 1fr;
      }
    }
    h1 {
      font-size: 40px;
      line-height: 1.1;
      margin: 0 0 16px;
    }
    p {
      margin: 0 0 12px;
      color: #c3c6d1;
    }
    .cta-row {
      margin-top: 20px;
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
    }
    .btn-primary {
      background: #007bff;
      color: #fff;
      border: none;
      padding: 12px 20px;
      border-radius: 999px;
      font-weight: 600;
      cursor: pointer;
    }
    .btn-secondary {
      background: transparent;
      color: #fff;
      border: 1px solid #3d4150;
      padding: 12px 20px;
      border-radius: 999px;
      font-weight: 500;
      cursor: pointer;
    }
    .grid-preview {
      background: radial-gradient(circle at top left, #1f2432, #0b0c10);
      border-radius: 16px;
      padding: 16px;
      border: 1px solid #262a38;
    }
    .grid-label {
      font-size: 12px;
      text-transform: uppercase;
      color: #9ea3b5;
      margin-bottom: 8px;
    }
    .mini-grid {
      display: grid;
      grid-template-columns: repeat(10, 1fr);
      gap: 2px;
      margin-top: 8px;
    }
    .mini-square {
      width: 16px;
      height: 16px;
      border-radius: 3px;
      background: #191b24;
    }
    .mini-square.selected {
      background: #007bff;
    }
    .mini-square.taken {
      background: #3b3f4f;
    }
    section {
      margin-top: 48px;
    }
    h2 {
      font-size: 24px;
      margin-bottom: 16px;
    }
    .steps {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 16px;
    }
    @media (max-width: 900px) {
      .steps {
        grid-template-columns: 1fr 1fr;
      }
    }
    @media (max-width: 600px) {
      .steps {
        grid-template-columns: 1fr;
      }
    }
    .step-card {
      background: #141621;
      border-radius: 12px;
      padding: 16px;
      border: 1px solid #242736;
    }
    .step-number {
      font-size: 12px;
      text-transform: uppercase;
      color: #ff8a00;
      margin-bottom: 4px;
    }
    .pill-row {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 8px;
    }
    .pill {
      font-size: 12px;
      padding: 4px 10px;
      border-radius: 999px;
      border: 1px solid #34384a;
      color: #bcc1d4;
    }
    footer {
      padding: 24px 16px;
      border-top: 1px solid #252732;
      text-align: center;
      font-size: 12px;
      color: #7e8294;
    }
    input[type="email"] {
      background: #141621;
      border-radius: 999px;
      border: 1px solid #34384a;
      padding: 10px 14px;
      color: #fff;
      min-width: 200px;
    }
  </style>
</head>
<body>
  <header>
    <div>
      <div class="logo">SQUORE BOX</div>
      <div class="tag">A winner a day, whenever we play</div>
    </div>
  </header>

  <main>
    <section class="hero">
      <div>
        <h1>Grid-based sports excitement with daily winners.</h1>
        <p>Squore Box is a 10×10 sports grid game tied to real basketball scores. Pick your squares, watch the game, and see who wins when the buzzer sounds.</p>
        <p>Built for fans who want simple, visual, and fair action every time they watch.</p>
        <div class="cta-row">
          <input type="email" placeholder="Enter your email to join the waitlist" />
          <button class="btn-primary">Join the waitlist</button>
          <button class="btn-secondary">See how it works</button>
        </div>
      </div>
      <div class="grid-preview">
        <div class="grid-label">Example Squore Box board · 10×10 grid</div>
        <div class="mini-grid">
          <!-- simple visual: some selected, some taken -->
          <!-- row 1 -->
          <div class="mini-square"></div>
          <div class="mini-square"></div>
          <div class="mini-square taken"></div>
          <div class="mini-square"></div>
          <div class="mini-square selected"></div>
          <div class="mini-square"></div>
          <div class="mini-square"></div>
          <div class="mini-square taken"></div>
          <div class="mini-square"></div>
          <div class="mini-square"></div>
          <!-- row 2 -->
          <div class="mini-square"></div>
          <div class="mini-square selected"></div>
          <div class="mini-square"></div>
          <div class="mini-square"></div>
          <div class="mini-square taken"></div>
          <div class="mini-square"></div>
          <div class="mini-square"></div>
          <div class="mini-square"></div>
          <div class="mini-square selected"></div>
          <div class="mini-square"></div>
          <!-- remaining squares -->
          <!-- you can leave the rest plain -->
          <!-- row 3-10 -->
          <!-- quick fill: 80 neutral squares -->
          <!-- generated quickly -->
          <!-- 80 divs -->
          <!-- you don't need to edit below to launch -->
          <!-- start bulk -->
          <div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div>
          <div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div>
          <div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div>
          <div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div>
          <div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div>
          <div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div>
          <div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div>
          <div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div><div class="mini-square"></div>
          <!-- end bulk -->
        </div>
        <p style="margin-top: 16px; font-size: 13px; color:#9ea3b5;">
          When the game ends, the last digit of each team’s score points to the winning square. Someone takes the prize every day we play.
        </p>
      </div>
    </section>

    <section>
      <h2>How Squore Box works</h2>
      <div class="steps">
        <div class="step-card">
          <div class="step-number">Step 1</div>
          <h3>Pick a board</h3>
          <p>Choose a board for today’s basketball game that matches your style and stakes.</p>
        </div>
        <div class="step-card">
          <div class="step-number">Step 2</div>
          <h3>Select your squares</h3>
          <p>Tap any spots on the 10×10 grid. Each square is a unique score combination.</p>
        </div>
        <div class="step-card">
          <div class="step-number">Step 3</div>
          <h3>Watch the game</h3>
          <p>Follow the action live while your squares ride along with every shot.</p>
        </div>
        <div class="step-card">
          <div class="step-number">Step 4</div>
          <h3>See who wins</h3>
          <p>When the buzzer sounds, the last digits of the final score reveal the winning square.</p>
        </div>
      </div>
    </section>

    <section>
      <h2>Why fans will love it</h2>
      <p>Squore Box is built for fans who want excitement without complexity. No confusing odds, no deep betting knowledge—just a clean grid, real scores, and guaranteed daily winners when games are played.</p>
      <div class="pill-row">
        <div class="pill">Daily winners</div>
        <div class="pill">Simple and visual</div>
        <div class="pill">Built for basketball</div>
        <div class="pill">Free-to-play first</div>
        <div class="pill">Ready for higher stakes where allowed</div>
      </div>
    </section>
  </main>

  <footer>
    © <span id="year"></span> Squore Box. Concept design in progress. Not a betting platform yet; features are subject to change.
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
