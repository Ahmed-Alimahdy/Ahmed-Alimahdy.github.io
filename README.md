# Ahmed-Alimahdy.github.io
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Ahmed Mahdy — Portfolio</title>
  <meta name="description" content="Portfolio of Ahmed Mahdy — frontend &amp; mobile developer">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; /* dark */
      --card:#0b1220;
      --muted:#94a3b8;
      --accent:#7c3aed;
      --glass: rgba(255,255,255,0.03);
      --radius:16px;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;padding:0;font-family:Inter,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;
      background:linear-gradient(180deg,#071025 0%, #081426 50%);color:#e6eef8;line-height:1.5;
      -webkit-font-smoothing:antialiased;
    }

    /* container */
    .wrap{max-width:1100px;margin:36px auto;padding:24px}

    /* header */
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#06b6d4);display:flex;align-items:center;justify-content:center;font-weight:800;color:white}
    nav{display:flex;gap:14px;align-items:center}
    nav a{color:var(--muted);text-decoration:none;padding:8px 10px;border-radius:10px}
    nav a:hover{color:white;background:rgba(255,255,255,0.03)}
    .cta{background:var(--accent);color:white;padding:8px 12px;border-radius:10px;text-decoration:none;font-weight:600}

    /* hero */
    .hero{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:center;margin-bottom:28px}
    .hero-left h1{margin:0;font-size:clamp(28px,4.5vw,44px)}
    .hero-left p{color:var(--muted);margin-top:8px}
    .skills{display:flex;flex-wrap:wrap;gap:8px;margin-top:18px}
    .skill{background:var(--glass);padding:8px 12px;border-radius:999px;color:var(--muted);font-size:14px}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.012));padding:18px;border-radius:var(--radius);box-shadow:0 6px 18px rgba(2,6,23,0.6)}
    .profile-pic{width:100%;border-radius:12px;display:block;object-fit:cover}

    /* projects */
    .section{margin-top:28px}
    .section h2{margin:0 0 12px 0}
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    .project{padding:16px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));border:1px solid rgba(255,255,255,0.02)}
    .project h3{margin:0 0 8px 0}
    .project p{margin:0;color:var(--muted);font-size:14px}
    .project a{display:inline-block;margin-top:10px;color:var(--accent);text-decoration:none;font-weight:600}

    /* contact */
    .contact-grid{display:grid;grid-template-columns:1fr 320px;gap:18px}
    label{display:block;font-size:13px;margin-bottom:6px;color:var(--muted)}
    input,textarea{width:100%;padding:10px;border-radius:10px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit}
    textarea{min-height:120px}
    button{background:var(--accent);border:none;padding:10px 14px;border-radius:10px;color:white;font-weight:700;cursor:pointer}

    footer{margin-top:36px;text-align:center;color:var(--muted);font-size:14px}

    /* responsiveness */
    @media (max-width:980px){
      .hero{grid-template-columns:1fr}
      .grid{grid-template-columns:repeat(2,1fr)}
      .contact-grid{grid-template-columns:1fr}
    }
    @media (max-width:560px){
      .grid{grid-template-columns:1fr}
      nav{display:none}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">AM</div>
        <div>
          <div style="font-weight:700">Ahmed Mahdy</div>
          <div style="font-size:13px;color:var(--muted)">Frontend & Mobile Developer</div>
        </div>
      </div>

      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
        <a class="cta" href="#contact">Hire me</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="hero-left">
          <h1>Hi — I'm Ahmed. I build clean, usable web & mobile apps.</h1>
          <p>I specialize in Flutter, Dart, and modern frontend workflows. I love turning ideas into polished, performant products.</p>
          <div class="skills">
            <span class="skill">Flutter</span>
            <span class="skill">Dart</span>
            <span class="skill">React</span>
            <span class="skill">TypeScript</span>
            <span class="skill">C++</span>
            <span class="skill">UI/UX</span>
          </div>

          <div style="margin-top:18px">
            <a class="cta" href="#projects" style="margin-right:10px">View projects</a>
            <a href="mailto:REPLACE_EMAIL" style="color:var(--muted);text-decoration:none">Email me</a>
          </div>
        </div>

        <aside class="card">
          <!-- Replace the image src with your photo or SVG -->
          <img class="profile-pic" src="REPLACE_PROFILE.jpg" alt="Ahmed Mahdy">
          <div style="margin-top:12px">
            <div style="font-weight:700">Ahmed Mahdy</div>
            <div style="font-size:13px;color:var(--muted)">Based in Cairo, Egypt • Open to remote</div>
          </div>
        </aside>
      </section>

      <section id="projects" class="section">
        <h2>Selected projects</h2>
        <div class="grid">
          <article class="project card">
            <h3>Expense Tracker (Flutter)</h3>
            <p>A clean cross-platform expense tracker with Cubit state management, persistent storage and intuitive keypad input.</p>
            <a href="#" target="_blank">View repo →</a>
          </article>

          <article class="project card">
            <h3>SimpleDigitalWallet (C++/CLI)</h3>
            <p>Windows Forms app integrating native C++ classes into managed UI for secure local wallet management.</p>
            <a href="#" target="_blank">View repo →</a>
          </article>

          <article class="project card">
            <h3>Machine Learning Pipeline</h3>
            <p>Preprocessing, feature selection and softmax regression implemented from scratch for anomaly detection experiments.</p>
            <a href="#" target="_blank">View repo →</a>
          </article>
        </div>
      </section>

      <section id="about" class="section">
        <h2>About me</h2>
        <div class="card" style="padding:20px">
          <p style="margin-top:0;color:var(--muted)">I'm a software engineer focused on building reliable and elegant user experiences. I enjoy working across the stack — from embedded C++ modules to polished Flutter frontends. Outside work I tinker with ML projects, teach myself new tools, and work out at the gym.</p>
          <p style="margin-top:12px">Want the full CV or references? <a href="REPLACE_CV.pdf" style="color:var(--accent);text-decoration:none">Download CV</a></p>
        </div>
      </section>

      <section id="contact" class="section">
        <h2>Contact</h2>
        <div class="contact-grid">
          <form class="card" onsubmit="event.preventDefault();alert('This is a demo contact form — replace with your backend or mailto link')">
            <label for="name">Name</label>
            <input id="name" placeholder="Your name">
            <label for="email">Email</label>
            <input id="email" placeholder="you@example.com">
            <label for="message">Message</label>
            <textarea id="message" placeholder="Tell me about your project"></textarea>
            <div style="margin-top:12px"><button type="submit">Send message</button></div>
          </form>

          <aside class="card" style="padding:18px">
            <h3 style="margin-top:0">Let's work together</h3>
            <p style="color:var(--muted)">Email: <a href="mailto:REPLACE_EMAIL" style="color:var(--accent);text-decoration:none">REPLACE_EMAIL</a></p>
            <p style="color:var(--muted)">GitHub: <a href="https://github.com/REPLACE_USERNAME" style="color:var(--accent);text-decoration:none">@REPLACE_USERNAME</a></p>
            <p style="color:var(--muted)">Location: Cairo, Egypt</p>
          </aside>
        </div>
      </section>
    </main>

    <footer>
      Built with ❤️ — Replace content and deploy to GitHub Pages
    </footer>
  </div>

  <script>
    // Small helper: replace placeholder profile image with a nice SVG if missing
    document.addEventListener('DOMContentLoaded',()=>{
      const img = document.querySelector('.profile-pic');
      if(img && img.getAttribute('src').includes('REPLACE')){
        img.src = 'data:image/svg+xml;utf8,' + encodeURIComponent(`<?xml version="1.0" encoding="UTF-8"?><svg xmlns="http://www.w3.org/2000/svg" width="800" height="600"><rect fill="#0b1220" width="100%" height="100%" rx="20"/><g fill="#c7d2fe" font-family="Inter, Arial" font-size="48"><text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle">AH</text></g></svg>`);
      }
    })
  </script>
</body>
</html>
