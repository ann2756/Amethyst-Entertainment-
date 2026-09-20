<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Amethyst Entertainment</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;600;700&family=DM+Sans:wght@400;500;600&family=Great+Vibes&display=swap" rel="stylesheet">

  <style>
    :root {
      --lavender: #ead7ff;
      --soft-purple: #cda4ff;
      --bright-purple: #a855f7;
      --deep-purple: #11001f;
      --card: rgba(25, 7, 48, 0.72);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      color: white;
      background:
        radial-gradient(circle at 15% 20%, rgba(168, 85, 247, 0.32), transparent 28%),
        radial-gradient(circle at 85% 15%, rgba(216, 164, 255, 0.2), transparent 24%),
        radial-gradient(circle at 50% 100%, rgba(124, 58, 237, 0.28), transparent 38%),
        linear-gradient(145deg, #08000f 0%, #19002e 45%, #2c0750 100%);
      background-attachment: fixed;
      min-height: 100vh;
      text-align: center;
      font-family: 'DM Sans', Arial, sans-serif;
      overflow-x: hidden;
      position: relative;
    }

    /* Soft decorative glow and stars */
    body::before,
    body::after {
      content: '✦  ·  ✧  ·  ✦';
      position: fixed;
      color: rgba(234, 215, 255, 0.5);
      font-size: 22px;
      letter-spacing: 22px;
      pointer-events: none;
      z-index: 0;
      animation: float 7s ease-in-out infinite;
    }

    body::before {
      top: 18%;
      left: 3%;
      text-shadow: 0 0 18px #d8a4ff;
    }

    body::after {
      right: 1%;
      bottom: 18%;
      transform: rotate(180deg);
      animation-delay: -3s;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-14px); }
    }

    header,
    .content,
    footer {
      position: relative;
      z-index: 1;
    }

    header {
      padding: 88px 20px 48px;
    }

    header::after {
      content: '';
      display: block;
      width: 130px;
      height: 2px;
      margin: 24px auto 0;
      background: linear-gradient(90deg, transparent, var(--soft-purple), transparent);
      box-shadow: 0 0 16px var(--bright-purple);
    }

    header h1 {
      color: #f6eaff;
      font-family: 'Great Vibes', cursive;
      font-size: clamp(3.6rem, 10vw, 6.8rem);
      font-weight: 400;
      line-height: 1;
      text-shadow: 0 0 10px #d8a4ff, 0 0 32px rgba(168, 85, 247, 0.9);
    }

    header p {
      margin-top: 18px;
      color: var(--lavender);
      font-family: 'Cinzel', serif;
      font-size: 0.95rem;
      letter-spacing: 3px;
      text-transform: uppercase;
    }

    .content {
      max-width: 850px;
      margin: auto;
      padding: 20px;
    }

    .card {
      background: linear-gradient(135deg, rgba(43, 13, 72, 0.82), var(--card));
      border: 1px solid rgba(225, 194, 255, 0.28);
      border-radius: 24px;
      padding: 38px 28px;
      margin-bottom: 25px;
      box-shadow: 0 10px 35px rgba(0, 0, 0, 0.35), inset 0 0 24px rgba(190, 125, 255, 0.08);
      backdrop-filter: blur(10px);
    }

    .card h2 {
      color: var(--soft-purple);
      font-family: 'Cinzel', serif;
      font-size: 1.55rem;
      letter-spacing: 2px;
      margin-bottom: 16px;
      text-shadow: 0 0 14px rgba(216, 164, 255, 0.65);
    }

    .card p {
      color: #f8eaff;
      line-height: 1.8;
      font-size: 1.02rem;
    }

    .members {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 12px;
      margin-top: 22px;
    }

    .member {
      background: linear-gradient(135deg, #7131a8, #a855f7);
      border: 1px solid rgba(255, 255, 255, 0.2);
      padding: 12px 19px;
      border-radius: 30px;
      font-weight: 600;
      box-shadow: 0 0 14px rgba(168, 85, 247, 0.3);
    }

    .social-links {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 14px;
      margin-top: 22px;
    }

    .social-links a {
      text-decoration: none;
      color: white;
      background: linear-gradient(135deg, #7e35b5, #a855f7);
      border: 1px solid rgba(255, 255, 255, 0.2);
      padding: 13px 22px;
      border-radius: 30px;
      font-weight: 600;
      transition: 0.3s ease;
      box-shadow: 0 0 14px rgba(168, 85, 247, 0.25);
    }

    .social-links a:hover {
      background: #e0b8ff;
      color: #26003e;
      transform: translateY(-4px);
      box-shadow: 0 0 24px rgba(216, 164, 255, 0.8);
    }

    footer {
      padding: 25px;
      color: #d9bced;
      font-size: 0.85rem;
    }

    @media (max-width: 600px) {
      header { padding-top: 65px; }
      header p { font-size: 0.75rem; letter-spacing: 1.5px; }
      .card { padding: 30px 20px; }
    }
  </style>
</head>

<body>
  <header>
    <h1>Amethyst Entertainment</h1>
    <p>Roblox entertainment inspired by KATSEYE</p>
  </header>

  <main class="content">
    <section class="card">
      <h2>About Us</h2>
      <p>
        Welcome to Amethyst Entertainment! We are a Roblox entertainment group
        inspired by the style, energy, and creativity of KATSEYE. Our goal is to
        create exciting performances, content, and unforgettable moments for
        our community.
      </p>
    </section>

    <section class="card">
      <h2>Our Members</h2>
      <p>All KATSEYE-inspired roles are currently taken.</p>

      <div class="members">
        <div class="member">Member 1</div>
        <div class="member">Member 2</div>
        <div class="member">Member 3</div>
        <div class="member">Member 4</div>
        <div class="member">Member 5</div>
        <div class="member">Member 6</div>
      </div>
    </section>

    <section class="card">
      <h2>Follow Us</h2>
      <p>Stay connected with Amethyst Entertainment.</p>

      <div class="social-links">
        <a href="https://www.roblox.com/" target="_blank" rel="noopener">Roblox</a>
        <a href="https://discord.com/" target="_blank" rel="noopener">Discord</a>
        <a href="https://www.tiktok.com/" target="_blank" rel="noopener">TikTok</a>
        <a href="https://www.youtube.com/" target="_blank" rel="noopener">YouTube</a>
        <a href="https://www.instagram.com/" target="_blank" rel="noopener">Instagram</a>
      </div>
    </section>
  </main>

  <footer>
    © 2026 Amethyst Entertainment. Created for Roblox entertainment.
    <br>
    Fan-inspired and not officially affiliated with KATSEYE.
  </footer>
</body>
</html>
