<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Bhoomika – GitHub Profile README</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet" />
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg: #0d0f14;
    --surface: #13161e;
    --surface2: #1a1e28;
    --border: rgba(255,255,255,0.07);
    --border2: rgba(255,255,255,0.12);
    --text: #eef0f6;
    --muted: #7b8099;
    --hint: #4a5068;
    --purple: #a78bfa;
    --purple-dim: rgba(167,139,250,0.12);
    --teal: #2dd4bf;
    --teal-dim: rgba(45,212,191,0.1);
    --amber: #fbbf24;
    --amber-dim: rgba(251,191,36,0.1);
    --pink: #f472b6;
    --pink-dim: rgba(244,114,182,0.1);
    --blue: #60a5fa;
    --blue-dim: rgba(96,165,250,0.1);
    --green: #86efac;
    --green-dim: rgba(134,239,172,0.1);
    --font: 'DM Sans', sans-serif;
    --mono: 'DM Mono', monospace;
  }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: var(--font);
    font-size: 15px;
    line-height: 1.6;
    padding: 2rem 1rem;
    min-height: 100vh;
  }

  .wrapper {
    max-width: 820px;
    margin: 0 auto;
    animation: fadeUp 0.6s ease both;
  }

  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(16px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  /* ── HERO ── */
  .hero {
    background: var(--surface);
    border: 1px solid var(--border2);
    border-radius: 20px;
    padding: 2.25rem 2rem;
    margin-bottom: 1.25rem;
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    top: -60px; right: -60px;
    width: 240px; height: 240px;
    background: radial-gradient(circle, rgba(167,139,250,0.15) 0%, transparent 70%);
    pointer-events: none;
  }

  .hero-top {
    display: flex;
    align-items: flex-start;
    gap: 1.25rem;
    margin-bottom: 1.25rem;
    flex-wrap: wrap;
  }

  .avatar {
    width: 72px; height: 72px;
    border-radius: 50%;
    background: linear-gradient(135deg, #7c3aed 0%, #0d9488 100%);
    display: flex; align-items: center; justify-content: center;
    font-size: 30px;
    flex-shrink: 0;
    box-shadow: 0 0 0 3px var(--bg), 0 0 0 5px rgba(167,139,250,0.3);
  }

  .hero-info { flex: 1; min-width: 200px; }

  .wave { display: inline-block; animation: wave 2.5s ease-in-out infinite; transform-origin: 70% 70%; }
  @keyframes wave {
    0%,100% { transform: rotate(0deg); }
    20% { transform: rotate(20deg); }
    40% { transform: rotate(-10deg); }
    60% { transform: rotate(15deg); }
    80% { transform: rotate(-5deg); }
  }

  .hero-name {
    font-size: 28px;
    font-weight: 600;
    color: var(--text);
    line-height: 1.2;
    margin-bottom: 4px;
  }

  .hero-title {
    font-size: 14px;
    color: var(--muted);
    font-family: var(--mono);
    margin-bottom: 1rem;
  }

  .badges {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .badge {
    font-size: 11.5px;
    font-weight: 500;
    padding: 4px 12px;
    border-radius: 20px;
    border: 1px solid transparent;
    white-space: nowrap;
  }

  .b-purple { background: var(--purple-dim); color: var(--purple); border-color: rgba(167,139,250,0.2); }
  .b-teal   { background: var(--teal-dim);   color: var(--teal);   border-color: rgba(45,212,191,0.2); }
  .b-amber  { background: var(--amber-dim);  color: var(--amber);  border-color: rgba(251,191,36,0.2); }
  .b-blue   { background: var(--blue-dim);   color: var(--blue);   border-color: rgba(96,165,250,0.2); }
  .b-pink   { background: var(--pink-dim);   color: var(--pink);   border-color: rgba(244,114,182,0.2); }
  .b-green  { background: var(--green-dim);  color: var(--green);  border-color: rgba(134,239,172,0.2); }

  .about {
    font-size: 14px;
    color: #a8b0c8;
    line-height: 1.7;
    margin-bottom: 1.25rem;
    padding-left: 0;
    max-width: 600px;
  }

  .links {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .link-btn {
    display: inline-flex;
    align-items: center;
    gap: 7px;
    font-size: 13px;
    font-weight: 500;
    padding: 7px 16px;
    border-radius: 10px;
    border: 1px solid var(--border2);
    color: var(--text);
    background: var(--surface2);
    text-decoration: none;
    transition: border-color 0.2s, background 0.2s, transform 0.15s;
  }

  .link-btn:hover {
    border-color: var(--border);
    background: rgba(255,255,255,0.05);
    transform: translateY(-1px);
  }

  .dot { width: 8px; height: 8px; border-radius: 50%; flex-shrink: 0; }

  /* ── SECTIONS ── */
  .section { margin-bottom: 1.25rem; }

  .section-title {
    font-size: 11px;
    font-weight: 600;
    color: var(--hint);
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-bottom: 0.75rem;
    font-family: var(--mono);
  }

  /* ── SKILL CARDS ── */
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
    gap: 10px;
  }

  .skill-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 14px 16px;
    transition: border-color 0.2s, transform 0.2s;
  }

  .skill-card:hover {
    border-color: var(--border2);
    transform: translateY(-2px);
  }

  .skill-header {
    display: flex;
    align-items: center;
    gap: 8px;
    margin-bottom: 10px;
  }

  .skill-icon {
    width: 30px; height: 30px;
    border-radius: 8px;
    display: flex; align-items: center; justify-content: center;
    font-size: 15px;
  }

  .skill-name {
    font-size: 13px;
    font-weight: 600;
    color: var(--text);
  }

  .skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 4px;
  }

  .skill-tag {
    font-size: 11px;
    color: var(--muted);
    background: var(--surface2);
    padding: 3px 9px;
    border-radius: 8px;
    border: 1px solid var(--border);
    font-family: var(--mono);
  }

  /* ── STATS ── */
  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
    gap: 10px;
  }

  .stat-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 14px;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }

  .stat-card img {
    width: 100%;
    border-radius: 6px;
    display: block;
  }

  /* ── DIVIDER ── */
  hr {
    border: none;
    border-top: 1px solid var(--border);
    margin: 1.25rem 0;
  }

  /* ── FOOTER ── */
  .footer {
    text-align: center;
    font-size: 12px;
    color: var(--hint);
    font-family: var(--mono);
    padding-top: 0.5rem;
  }

  .footer span { color: var(--purple); }

  /* ── RESPONSIVE ── */
  @media (max-width: 560px) {
    .hero { padding: 1.5rem 1.25rem; }
    .hero-name { font-size: 22px; }
    .skills-grid, .stats-grid { grid-template-columns: 1fr; }
  }
</style>
</head>
<body>

<div class="wrapper">

  <!-- HERO -->
  <div class="hero">
    <div class="hero-top">
      <div class="avatar">👩‍💻</div>
      <div class="hero-info">
        <div class="hero-name"><span class="wave">👋</span> Hi, I'm Bhoomika!</div>
        <div class="hero-title">software_engineer.py · ai_ml_enthusiast.py</div>
        <div class="badges">
          <span class="badge b-purple">M.S. · University at Buffalo '26</span>
          <span class="badge b-teal">Backend Systems</span>
          <span class="badge b-blue">AI / ML</span>
          <span class="badge b-amber">⚡ Open to Work</span>
        </div>
      </div>
    </div>

    <p class="about">
      Building scalable backend systems, intelligent applications, and ML platforms.
      I love turning complex problems into clean, performant code — from distributed systems to deep learning pipelines.
    </p>

    <div class="links">
      <a class="link-btn" href="mailto:bhoomikakoratee@gmail.com">
        <span class="dot" style="background:#f87171;"></span> Email
      </a>
      <a class="link-btn" href="https://github.com/bhoomikajagadeesh">
        <span class="dot" style="background:#a78bfa;"></span> GitHub
      </a>
      <a class="link-btn" href="https://www.linkedin.com/in/bhoomikakjkora">
        <span class="dot" style="background:#60a5fa;"></span> LinkedIn
      </a>
      <a class="link-btn" href="https://leetcode.com/u/bhoomikakj/">
        <span class="dot" style="background:#fbbf24;"></span> LeetCode
      </a>
    </div>
  </div>

  <!-- SKILLS -->
  <div class="section">
    <div class="section-title">// Skills &amp; Technologies</div>
    <div class="skills-grid">

      <div class="skill-card">
        <div class="skill-header">
          <div class="skill-icon" style="background:rgba(167,139,250,0.12);">⚡</div>
          <span class="skill-name">Frontend</span>
        </div>
        <div class="skill-tags">
          <span class="skill-tag">React</span>
          <span class="skill-tag">Angular</span>
          <span class="skill-tag">Vue.js</span>
          <span class="skill-tag">HTML5</span>
          <span class="skill-tag">CSS3</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-header">
          <div class="skill-icon" style="background:rgba(45,212,191,0.1);">🔧</div>
          <span class="skill-name">Backend</span>
        </div>
        <div class="skill-tags">
          <span class="skill-tag">Node.js</span>
          <span class="skill-tag">NestJS</span>
          <span class="skill-tag">Spring</span>
          <span class="skill-tag">Express</span>
          <span class="skill-tag">Kafka</span>
          <span class="skill-tag">Nginx</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-header">
          <div class="skill-icon" style="background:rgba(244,114,182,0.1);">🤖</div>
          <span class="skill-name">AI &amp; ML</span>
        </div>
        <div class="skill-tags">
          <span class="skill-tag">TensorFlow</span>
          <span class="skill-tag">PyTorch</span>
          <span class="skill-tag">scikit-learn</span>
          <span class="skill-tag">HuggingFace</span>
          <span class="skill-tag">OpenCV</span>
          <span class="skill-tag">Pandas</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-header">
          <div class="skill-icon" style="background:rgba(96,165,250,0.1);">🗄️</div>
          <span class="skill-name">Databases</span>
        </div>
        <div class="skill-tags">
          <span class="skill-tag">PostgreSQL</span>
          <span class="skill-tag">MongoDB</span>
          <span class="skill-tag">MySQL</span>
          <span class="skill-tag">Redis</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-header">
          <div class="skill-icon" style="background:rgba(251,191,36,0.1);">☁️</div>
          <span class="skill-name">DevOps &amp; Cloud</span>
        </div>
        <div class="skill-tags">
          <span class="skill-tag">Docker</span>
          <span class="skill-tag">Kubernetes</span>
          <span class="skill-tag">AWS</span>
          <span class="skill-tag">GCP</span>
          <span class="skill-tag">Jenkins</span>
          <span class="skill-tag">Firebase</span>
          <span class="skill-tag">Postman</span>
        </div>
      </div>

    </div>
  </div>

  <hr />

  <!-- STATS -->
  <div class="section">
    <div class="section-title">// GitHub Stats</div>
    <div class="stats-grid">
      <div class="stat-card">
        <img
          src="https://github-readme-stats.vercel.app/api/top-langs?username=bhoomikajagadeesh&layout=compact&theme=tokyonight&hide_border=true&bg_color=13161e&title_color=a78bfa&text_color=7b8099"
          alt="Top Languages"
        />
      </div>
      <div class="stat-card">
        <img
          src="https://github-readme-stats.vercel.app/api?username=bhoomikajagadeesh&show_icons=true&theme=tokyonight&hide_border=true&bg_color=13161e&title_color=a78bfa&icon_color=2dd4bf&text_color=7b8099"
          alt="GitHub Stats"
        />
      </div>
      <div class="stat-card">
        <img
          src="https://github-readme-streak-stats.herokuapp.com/?user=bhoomikajagadeesh&theme=tokyonight&hide_border=true&background=13161e&ring=a78bfa&fire=fbbf24&currStreakLabel=a78bfa"
          alt="Streak Stats"
        />
      </div>
    </div>
  </div>

  <div class="footer">
    made with <span>♥</span> · bhoomika jagadeesh
  </div>

</div>
</body>
</html>
