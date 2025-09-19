<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Ahmed Mahdy — Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724;
      --muted:#94a3b8;
      --accent:#7c3aed;
      --glass: rgba(255,255,255,0.03);
      --radius:20px;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family:Inter,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;
      background:linear-gradient(180deg,#071025 0%, #081426 50%);
      color:#e6eef8;
      line-height:1.6;
    }

    .wrap{max-width:1200px;margin:0 auto;padding:48px 24px;animation:fadeIn 1.2s ease-in}

    @keyframes fadeIn{
      from{opacity:0;transform:translateY(20px)}
      to{opacity:1;transform:translateY(0)}
    }

    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:64px;animation:slideDown 1s ease-out}
    @keyframes slideDown{
      from{opacity:0;transform:translateY(-40px)}
      to{opacity:1;transform:translateY(0)}
    }

    .brand{display:flex;gap:16px;align-items:center}
    .logo-img{width:64px;height:64px;border-radius:16px;object-fit:cover;animation:pulse 2s infinite alternate}
    @keyframes pulse{
      from{transform:scale(1)}
      to{transform:scale(1.08)}
    }

    nav{display:flex;gap:20px;align-items:center}
    nav a{color:var(--muted);text-decoration:none;padding:10px 14px;border-radius:12px;font-size:15px;transition:all .3s}
    nav a:hover{color:white;background:rgba(255,255,255,0.05);transform:translateY(-2px)}
    .cta{background:var(--accent);color:white;padding:10px 16px;border-radius:12px;text-decoration:none;font-weight:600;transition:all .3s}
    .cta:hover{background:#9f67ff;transform:scale(1.05)}

    .hero{display:grid;grid-template-columns:1fr 400px;gap:40px;align-items:center;margin-bottom:72px}
    .hero-left h1{margin:0;font-size:clamp(32px,4.5vw,50px);line-height:1.3;animation:fadeInUp 1.5s ease}
    @keyframes fadeInUp{
      from{opacity:0;transform:translateY(30px)}
      to{opacity:1;transform:translateY(0)}
    }
    .hero-left p{color:var(--muted);margin-top:16px;font-size:18px}
    .skills{display:flex;flex-wrap:wrap;gap:12px;margin-top:24px}
    .skill{background:var(--glass);padding:10px 16px;border-radius:999px;color:var(--muted);font-size:15px;transition:all .3s}
    .skill:hover{background:var(--accent);color:white;transform:translateY(-3px)}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:28px;border-radius:var(--radius);box-shadow:0 8px 24px rgba(2,6,23,0.7);transition:transform .3s, box-shadow .3s}
    .card:hover{transform:translateY(-6px);box-shadow:0 12px 28px rgba(2,6,23,0.9)}
    .profile-pic{width:100%;border-radius:16px;object-fit:cover;animation:fadeIn 2s ease}

    .section{margin-top:80px}
    .section h2{margin:0 0 24px 0;font-size:28px;animation:fadeInUp 1s ease}
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:28px}
    .project{padding:24px;border-radius:16px;background:linear-gradient(180deg, rgba(255,255,255,0.015), rgba(255,255,255,0.005));border:1px solid rgba(255,255,255,0.04)}
    .project h3{margin:0 0 12px 0;font-size:20px}
    .project p{margin:0;color:var(--muted);font-size:15px}
    .project a{display:inline-block;margin-top:14px;color:var(--accent);text-decoration:none;font-weight:600;transition:color .3s}
    .project a:hover{color:#a78bfa}

    .contact-grid{display:grid;grid-template-columns:1fr 360px;gap:28px}
    input,textarea{width:100%;padding:14px;border-radius:12px;border:1px solid rgba(255,255,255,0.05);background:transparent;color:inherit;font-size:15px;transition:border .3s}
    input:focus,textarea:focus{border-color:var(--accent);outline:none}
    button{background:var(--accent);border:none;padding:12px 18px;border-radius:12px;color:white;font-weight:700;cursor:pointer;transition:background .3s,transform .2s}
    button:hover{background:#9f67ff;transform:scale(1.05)}
    .project-card {
  overflow: hidden; /* يخلي الصورة ما تطلعش برا الكارت */
}

.project-img {
  width: 100%;           /* تخليها تاخد عرض الكارت */
  height: 200px;         /* ارتفاع ثابت (تقدر تزوده أو تقلله) */
  object-fit: contain;   /* تعمل Zoom out بحيث الصورة كاملة تظهر */
  object-position: center; /* توسيط الصورة داخل الكارت */
}

    footer{margin-top:72px;text-align:center;color:var(--muted);font-size:15px;animation:fadeIn 2s ease-in}

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
        <img src="C:\Users\Ahmed Ali\Desktop\WhatsApp Image 2025-09-10 at 18.15.34_b8cd6d06.jpg" alt="Logo" class="logo-img">
        <div>
          <div style="font-weight:700;font-size:18px">Ahmed Mahdy</div>
          <div style="font-size:14px;color:var(--muted)">Cross platform Mobile Developer (Flutter) & Software engineering</div>
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
          <p>I specialize in Flutter, Dart, and modern frontend workflows. turning ideas into polished, performant products.</p>
          <div class="skills">
            <span class="skill">Flutter</span>
            <span class="skill">Dart</span>
            <span class="skill">SQflite</span>
            <span class="skill">Json</span>
            <span class="skill">API integration</span>
            <span class="skill">animation</span>
            <span class="skill">Java</span>
            <span class="skill">C++</span>
            <span class="skill">ASP.net</span>
            <span class="skill">UI/UX</span>
          </div>
          <div style="margin-top:28px">
            <a class="cta" href="#projects" style="margin-right:16px">View projects</a>
            <a href="mailto:ahmed.almahdy005@gmail.com" style="color:var(--muted);text-decoration:none;font-size:15px">Email me</a>
          </div>
        </div>
        <aside class="card">
          <img class="profile-pic" src="C:\Users\Ahmed Ali\Desktop\Screenshot 2025-09-11 012207.png" alt="Ahmed Mahdy">
          <div style="margin-top:16px">
            <div style="font-weight:700;font-size:18px">Ahmed Mahdy</div>
            <div style="font-size:14px;color:var(--muted)">Based in Cairo, Egypt • Open to remote</div>
          </div>
        </aside>
      </section>

 <section id="projects" class="section">
  <h2>Projects</h2>
  <div class="grid">

    <div class="card project-card">
      <img src="C:\Users\Ahmed AliScreenshot 2025-08-24 232800.png" alt="Expense Tracker App screenshot" class="project-img">
      <h3>Expense Tracker App</h3>
      <p>A Flutter app to track expenses with charts, categories, and a clean UI.</p>
      <a href="https://github.com/Ahmed-Alimahdy/expense_tracker" target="_blank" class="btn">View Project</a>
    </div>

  
    <div class="card project-card">
      <img src="C:\Users\Ahmed Ali\OneDrive\Pictures\Screenshots\Screenshot 2025-08-24 232800.png" alt="Quotify App screenshot" class="project-img">
      <h3>Quotify</h3>
      <p>A Flutter application for generating random quotes</p>
      <a href="https://github.com/Ahmed-Alimahdy/Quotify" target="_blank" class="btn">View Project</a>
    </div>

  

  </div>
</section>


      <section id="about" class="section">
        <h2>About me</h2>
        <div class="card" style="padding:28px">
          <p style="margin-top:0;color:var(--muted);font-size:16px">I am Flutter app developer, creating applications for multiple operating systems like Android and iOS — from the initial idea to a fully complete service. I started learning and became passionate about Flutter after gaining several experiences in AI and web development. Then, I began creating my own custom mobile applications to track my progress in real life and take notes along the way</p>
          <p style="margin-top:20px;font-size:16px">Want the full CV or references? <a href="C:\Users\Ahmed Ali\Desktop\Ahmed Ali Mahdy.pdf" style="color:var(--accent);text-decoration:none">Download CV</a></p>
        </div>
      </section>

     <section id="contact" class="section">
  <h2>Contact</h2>
  <div class="contact-grid">
    
    <!-- Contact Form -->
    <form id="contact-form" action="https://formspree.io/f/xzzaooqb" method="POST" class="card">
      <label for="name">Name</label>
      <input id="name" type="text" name="name" required placeholder="Your name">

      <label for="email">Email</label>
      <input id="email" type="email" name="_replyto" required placeholder="you@example.com">

      <label for="message">Message</label>
      <textarea id="message" name="message" required placeholder="Tell me about your project"></textarea>

      <input type="hidden" name="_subject" value="New Portfolio Message">

      <div style="margin-top:20px">
        <button type="submit">Send message</button>
      </div>
    </form>

    <!-- Success message -->
    <p id="status-msg" style="display:none; color: lightgreen; margin-top:15px; font-weight: bold; transition: opacity 0.5s;">
      ✅ Thanks! Your message has been sent.
    </p>

    <!-- Contact Info Card -->
    <aside class="card" style="padding:24px">
      <h3 style="margin-top:0">Let's work together</h3>
      <p style="color:var(--muted);font-size:15px">
        Email: <a href="mailto:ahmed.almahdy005@gmail.com" style="color:var(--accent);text-decoration:none">ahmed.almahdy005@gmail.com</a>
      </p>
      <p style="color:var(--muted);font-size:15px">
        GitHub: <a href="https://github.com/Ahmed-Alimahdy" style="color:var(--accent);text-decoration:none">Ahmed-Alimahdy</a>
      </p>
      <p style="color:var(--muted);font-size:15px">
        WhatsApp: <a style="color:var(--accent);text-decoration:none">01204823840</a>
      </p>
      <p style="color:var(--muted);font-size:15px">Location: Cairo, Egypt</p>
    </aside>
  </div>
</section>

<!-- Form Handler -->
<script>
  const form = document.getElementById("contact-form");
  const statusMsg = document.getElementById("status-msg");

  form.addEventListener("submit", async function(e) {
    e.preventDefault();

    const formData = new FormData(form);

    try {
      const response = await fetch(form.action, {
        method: form.method,
        body: formData,
        headers: { 'Accept': 'application/json' }
      });

      if (response.ok) {
        form.reset(); // clear fields
        statusMsg.style.display = "block";
        statusMsg.style.opacity = "1";

        // hide message smoothly after 5s
        setTimeout(() => {
          statusMsg.style.opacity = "0";
        }, 5000);
      } else {
        alert("Oops! Something went wrong. Please try again.");
      }
    } catch (error) {
      alert("Failed to send message. Please check your connection.");
    }
  });
</script>

<!-- Contact Grid Styles -->
<style>
  .contact-grid {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 24px;
    align-items: start;
  }

  @media (max-width: 768px) {
    .contact-grid {
      grid-template-columns: 1fr; 
    }
  }
</style>

    </main>
  </div>
</body>
</html>
