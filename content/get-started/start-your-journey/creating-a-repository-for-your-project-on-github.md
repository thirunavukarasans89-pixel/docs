
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#080b14">
  <title>STVK | Creative Portfolio</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      background: #080b14;
      color: #f4f7ff;
      line-height: 1.7;
    }

    :root {
      --blue: #42a5ff;
      --panel: #111827;
      --muted: #a5b1c8;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 10;
      background: #080b14ee;
      border-bottom: 1px solid #253149;
      padding: 14px 5%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
    }

    .logo {
      color: var(--blue);
      font-size: 25px;
      font-weight: 900;
      letter-spacing: 3px;
    }

    nav {
      display: flex;
      flex-wrap: wrap;
      gap: 13px;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-size: 13px;
    }

    nav a:hover {
      color: var(--blue);
    }

    section {
      padding: 65px 7%;
      scroll-margin-top: 65px;
    }

    .hero {
      min-height: 82vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: flex-start;
      background:
        radial-gradient(ellipse at 90% 20%,
        #12376a 0%, transparent 45%);
    }

    .tag {
      color: var(--blue);
      letter-spacing: 3px;
      font-size: 12px;
      font-weight: bold;
    }

    h1 {
      font-size: clamp(52px, 12vw, 92px);
      line-height: 1.15;
      margin: 12px 0;
    }

    h1 span, h2 span {
      color: var(--blue);
    }

    .hero p, .about p {
      max-width: 580px;
      color: var(--muted);
      margin: 12px 0 25px;
    }

    .btn {
      display: inline-block;
      padding: 11px 20px;
      border-radius: 7px;
      background: var(--blue);
      color: #06101f;
      text-decoration: none;
      font-weight: bold;
      border: 0;
      cursor: pointer;
      margin: 5px 5px 5px 0;
    }

    .btn.secondary {
      color: white;
      background: transparent;
      border: 1px solid var(--blue);
    }

    h2 {
      font-size: 34px;
      margin-bottom: 12px;
    }

    .subtitle {
      color: var(--muted);
      margin-bottom: 25px;
    }

    .panel {
      background: var(--panel);
      padding: 24px;
      border: 1px solid #253149;
      border-radius: 14px;
    }

    .skills, .gallery {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 15px;
      margin-top: 22px;
    }

    .skill {
      background: var(--panel);
      padding: 18px;
      border-radius: 10px;
      border: 1px solid #253149;
    }

    .art {
      min-height: 145px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 43px;
      background: linear-gradient(135deg, #102b50, #17132c);
      border-radius: 9px;
      margin-bottom: 12px;
    }

    .project {
      background: var(--panel);
      border: 1px solid #253149;
      border-radius: 12px;
      padding: 12px;
      overflow: hidden;
    }

    .project h3 {
      font-size: 16px;
    }

    .project p {
      color: var(--muted);
      font-size: 13px;
    }

    .contact-links {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 18px;
    }

    footer {
      text-align: center;
      color: var(--muted);
      border-top: 1px solid #253149;
      padding: 22px 12px;
      font-size: 13px;
    }

    @media (min-width: 700px) {
      .skills, .gallery {
        grid-template-columns: repeat(3, minmax(0, 1fr));
      }
    }

    @media (max-width: 380px) {
      header {
        align-items: flex-start;
        flex-direction: column;
      }
      nav {
        gap: 10px;
      }
      section {
        padding: 48px 5%;
      }
    }
  </style>
</head>

<body>
  <header>
    <div class="logo">STVK.</div>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#work">My Work</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="tag">WELCOME TO MY WORLD</div>
      <h1>I'm <span>STVK</span></h1>
      <h2>Artist. Creator. <span>Dreamer.</span></h2>
      <p>
        Welcome to my creative portfolio.
        Explore my drawings, designs, ideas,
        and projects all in one place.
      </p>
      <div>
        <a class="btn" href="#work">Explore My Work ↗</a>
        <a class="btn secondary" href="#contact">Contact Me</a>
      </div>
    </section>

    <section id="about" class="about">
      <div class="tag">GET TO KNOW ME</div>
      <h2>About <span>Me</span></h2>
      <div class="panel">
        <p>
          Hi! I'm STVK, a creative person who loves
          art, drawing, design, and digital creativity.
          I enjoy turning ideas into visuals and
          learning new skills through every project.
        </p>
        <p>
          This website is my personal space to
          showcase my creations and creative journey.
        </p>
      </div>
    </section>

    <section id="skills">
      <div class="tag">WHAT I LOVE</div>
      <h2>My <span>Skills</span></h2>
      <p class="subtitle">Things I enjoy creating and learning.</p>

      <div class="skills">
        <div class="skill">✏️ <h3>Drawing</h3>
          <p>Sketches and original artwork.</p></div>
        <div class="skill">🎨 <h3>Digital Art</h3>
          <p>Creative visuals and compositions.</p></div>
        <div class="skill">💻 <h3>Web Design</h3>
          <p>Learning to build websites.</p></div>
        <div class="skill">✨ <h3>Photo Editing</h3>
          <p>Effects, lighting, and posters.</p></div>
      </div>
    </section>

    <section id="work">
      <div class="tag">MY CREATIONS</div>
      <h2>Featured <span>Work</span></h2>
      <p class="subtitle">
        Replace these sample cards with your real artwork.
      </p>

      <div class="gallery">
        <article class="project">
          <div class="art">✏️</div>
          <h3>Pencil Sketches</h3>
          <p>Hand-drawn artwork</p>
        </article>

        <article class="project">
          <div class="art">🌌</div>
          <h3>Digital Art</h3>
          <p>Creative digital designs</p>
        </article>

        <article class="project">
          <div class="art">⚡</div>
          <h3>Poster Designs</h3>
          <p>Bold and cinematic edits</p>
        </article>

        <article class="project">
          <div class="art">🦋</div>
          <h3>Creative Concepts</h3>
          <p>Ideas and experiments</p>
        </article>

        <article class="project">
          <div class="art">🌙</div>
          <h3>Photography</h3>
          <p>Light, mood, and atmosphere</p>
        </article>

        <article class="project">
          <div class="art">💙</div>
          <h3>More Projects</h3>
          <p>My ongoing creative journey</p>
        </article>
      </div>
    </section>

    <section id="contact">
      <div class="tag">LET'S CONNECT</div>
      <h2>Contact <span>Me</span></h2>
      <div class="panel">
        <p>
          Thanks for visiting my portfolio!
          You can find my work and follow my
          creative journey through my social links.
        </p>

        <div class="contact-links">
          <!-- Replace # with your real profile URLs -->
          <a class="btn" href="#"
             onclick="return profileNotice(event)">
             Instagram ↗
          </a>
          <a class="btn secondary" href="#"
             onclick="return profileNotice(event)">
             YouTube ↗
          </a>
        </div>
      </div>
    </section>
  </main>

  <footer>
    © <span id="year"></span> STVK. Made with 💙
  </footer>

  <script>
    document.getElementById("year").textContent =
      new Date().getFullYear();

    function profileNotice(event) {
      event.preventDefault();
      alert("Add your social profile URL in the HTML code first!");
      return false;
    }
  </script>
</body>
</html>
