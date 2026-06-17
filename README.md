
<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=Space+Mono:wght@400;700&display=swap');

  * { box-sizing: border-box; margin: 0; padding: 0; }

  .readme {
    background: #0a0a0a;
    color: #e8e8e2;
    font-family: 'Space Grotesk', sans-serif;
    padding: 48px 40px;
    border-radius: 12px;
    border: 0.5px solid #222;
    min-height: 100vh;
  }

  .mono { font-family: 'Space Mono', monospace; }

  .hero {
    text-align: center;
    padding: 40px 0 56px;
    border-bottom: 0.5px solid #1e1e1e;
    margin-bottom: 56px;
  }

  .logotype {
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    color: #00ff9f;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    margin-bottom: 32px;
    opacity: 0.7;
  }

  .hero-name {
    font-size: 64px;
    font-weight: 700;
    letter-spacing: -2px;
    line-height: 1;
    color: #f0f0ea;
    margin-bottom: 16px;
  }

  .hero-name span { color: #00ff9f; }

  .hero-tagline {
    font-size: 14px;
    color: #555;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    font-family: 'Space Mono', monospace;
    margin-bottom: 40px;
  }

  .badge-row {
    display: flex;
    gap: 10px;
    justify-content: center;
    flex-wrap: wrap;
  }

  .badge {
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    padding: 7px 16px;
    border: 0.5px solid #333;
    border-radius: 2px;
    color: #888;
    text-decoration: none;
    letter-spacing: 0.1em;
    transition: border-color 0.2s, color 0.2s;
    cursor: pointer;
  }
  .badge:hover { border-color: #00ff9f; color: #00ff9f; }

  .section {
    margin-bottom: 64px;
  }

  .section-label {
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    color: #00ff9f;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    margin-bottom: 24px;
    display: flex;
    align-items: center;
    gap: 16px;
  }
  .section-label::after {
    content: '';
    flex: 1;
    height: 0.5px;
    background: #1e1e1e;
  }

  .section-title {
    font-size: 28px;
    font-weight: 600;
    color: #f0f0ea;
    margin-bottom: 12px;
    letter-spacing: -0.5px;
  }

  .section-sub {
    font-size: 14px;
    color: #555;
    line-height: 1.7;
    max-width: 520px;
    margin-bottom: 32px;
  }

  .service-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1px;
    background: #1a1a1a;
    border: 0.5px solid #1a1a1a;
    border-radius: 6px;
    overflow: hidden;
  }

  .service-card {
    background: #0d0d0d;
    padding: 28px 24px;
  }

  .service-icon {
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    color: #00ff9f;
    letter-spacing: 0.2em;
    margin-bottom: 16px;
  }

  .service-name {
    font-size: 15px;
    font-weight: 600;
    color: #e8e8e2;
    margin-bottom: 8px;
  }

  .service-desc {
    font-size: 12px;
    color: #444;
    line-height: 1.7;
  }

  .stack-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1px;
    background: #1a1a1a;
    border: 0.5px solid #1a1a1a;
    border-radius: 6px;
    overflow: hidden;
  }

  .stack-row {
    background: #0d0d0d;
    padding: 18px 24px;
    display: flex;
    gap: 16px;
    align-items: flex-start;
  }

  .stack-cat {
    font-family: 'Space Mono', monospace;
    font-size: 9px;
    color: #00ff9f;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    min-width: 80px;
    padding-top: 2px;
  }

  .stack-pills {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .pill {
    font-size: 11px;
    color: #777;
    background: #141414;
    border: 0.5px solid #2a2a2a;
    border-radius: 2px;
    padding: 3px 10px;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1px;
    background: #1a1a1a;
    border: 0.5px solid #1a1a1a;
    border-radius: 6px;
    overflow: hidden;
    margin-bottom: 32px;
  }

  .stat-box {
    background: #0d0d0d;
    padding: 28px 20px;
    text-align: center;
  }

  .stat-num {
    font-family: 'Space Mono', monospace;
    font-size: 32px;
    font-weight: 700;
    color: #00ff9f;
    line-height: 1;
    margin-bottom: 8px;
  }

  .stat-label {
    font-size: 11px;
    color: #444;
    letter-spacing: 0.1em;
    text-transform: uppercase;
  }

  .process-row {
    display: flex;
    gap: 0;
    margin-bottom: 8px;
  }

  .process-step {
    flex: 1;
    background: #0d0d0d;
    border: 0.5px solid #1a1a1a;
    padding: 20px 18px;
    position: relative;
  }

  .process-step:first-child { border-radius: 6px 0 0 6px; }
  .process-step:last-child { border-radius: 0 6px 6px 0; }

  .process-num {
    font-family: 'Space Mono', monospace;
    font-size: 9px;
    color: #333;
    margin-bottom: 10px;
  }

  .process-title {
    font-size: 12px;
    font-weight: 600;
    color: #e8e8e2;
    margin-bottom: 6px;
  }

  .process-items {
    font-size: 11px;
    color: #3a3a3a;
    line-height: 1.8;
    list-style: none;
  }

  .process-items li::before {
    content: '— ';
    color: #00ff9f;
  }

  .arrow-connector {
    display: flex;
    align-items: center;
    padding: 0 4px;
    color: #2a2a2a;
    font-size: 18px;
    font-weight: 300;
  }

  .quote-block {
    border-left: 1px solid #00ff9f;
    padding: 16px 24px;
    background: #0d0d0d;
    border-radius: 0 6px 6px 0;
    margin-bottom: 12px;
  }

  .quote-text {
    font-size: 14px;
    color: #888;
    font-style: italic;
    line-height: 1.7;
    margin-bottom: 10px;
  }

  .quote-attr {
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    color: #333;
    letter-spacing: 0.1em;
  }

  .cta-block {
    background: #0d0d0d;
    border: 0.5px solid #1e1e1e;
    border-radius: 6px;
    padding: 40px;
    text-align: center;
  }

  .cta-eyebrow {
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    color: #333;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    margin-bottom: 16px;
  }

  .cta-headline {
    font-size: 28px;
    font-weight: 600;
    color: #f0f0ea;
    margin-bottom: 8px;
    letter-spacing: -0.5px;
  }

  .cta-sub {
    font-size: 13px;
    color: #444;
    margin-bottom: 32px;
  }

  .cta-buttons {
    display: flex;
    gap: 12px;
    justify-content: center;
    flex-wrap: wrap;
  }

  .btn-primary {
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.1em;
    padding: 13px 28px;
    background: #00ff9f;
    color: #000;
    border: none;
    border-radius: 2px;
    cursor: pointer;
    text-transform: uppercase;
    font-weight: 700;
  }

  .btn-secondary {
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.1em;
    padding: 13px 28px;
    background: transparent;
    color: #555;
    border: 0.5px solid #2a2a2a;
    border-radius: 2px;
    cursor: pointer;
    text-transform: uppercase;
  }

  .footer-line {
    text-align: center;
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    color: #2a2a2a;
    margin-top: 48px;
    letter-spacing: 0.2em;
    padding-top: 24px;
    border-top: 0.5px solid #111;
  }

  .divider { height: 0.5px; background: #1a1a1a; margin: 0 0 56px; }
</style>

<div class="readme">

  <div class="hero">
    <div class="logotype mono">Next-Gen Software Agency &nbsp;·&nbsp; Est. 2024</div>
    <div class="hero-name">SYNT<span>AX</span>O</div>
    <div class="hero-tagline">We engineer competitive advantages</div>
    <div class="badge-row">
      <a class="badge" href="https://syntaxo.shvx.dev">↗ syntaxo.shvx.dev</a>
      <a class="badge" href="mailto:hello@syntaxo.tech">✉ hello@syntaxo.tech</a>
      <a class="badge" href="https://x.com/syntax_o_tech">𝕏 @syntax_o_tech</a>
    </div>
  </div>

  <div class="section">
    <div class="section-label">01 — Services</div>
    <div class="section-title">What we build</div>
    <div class="section-sub">We partner with ambitious teams to ship software that performs at scale. No bloat. No hand-holding. Just precision engineering.</div>
    <div class="service-grid">
      <div class="service-card">
        <div class="service-icon">AI / AUTO</div>
        <div class="service-name">AI & Automation</div>
        <div class="service-desc">Production-grade LLM agents, workflow automation, and multi-model pipelines that run your operations — not just assist them.</div>
      </div>
      <div class="service-card">
        <div class="service-icon">SAAS / WEB</div>
        <div class="service-name">SaaS & Web Apps</div>
        <div class="service-desc">High-throughput web platforms built for real traffic. From zero-to-launch MVPs to full-scale overhauls — engineered to perform.</div>
      </div>
      <div class="service-card">
        <div class="service-icon">iOS / ANDROID</div>
        <div class="service-name">Mobile Apps</div>
        <div class="service-desc">Native-feel iOS & Android, architected for retention. The obsessive UX detail that keeps users coming back.</div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">02 — Stack</div>
    <div class="stack-grid">
      <div class="stack-row">
        <div class="stack-cat">Frontend</div>
        <div class="stack-pills">
          <span class="pill">React</span><span class="pill">Next.js</span><span class="pill">TypeScript</span><span class="pill">Tailwind</span>
        </div>
      </div>
      <div class="stack-row">
        <div class="stack-cat">Backend</div>
        <div class="stack-pills">
          <span class="pill">Node.js</span><span class="pill">Python</span><span class="pill">FastAPI</span><span class="pill">GraphQL</span>
        </div>
      </div>
      <div class="stack-row">
        <div class="stack-cat">Data</div>
        <div class="stack-pills">
          <span class="pill">PostgreSQL</span><span class="pill">MongoDB</span><span class="pill">Redis</span><span class="pill">Supabase</span>
        </div>
      </div>
      <div class="stack-row">
        <div class="stack-cat">AI / ML</div>
        <div class="stack-pills">
          <span class="pill">OpenAI</span><span class="pill">Anthropic</span><span class="pill">LangChain</span><span class="pill">Pinecone</span>
        </div>
      </div>
      <div class="stack-row">
        <div class="stack-cat">Infra</div>
        <div class="stack-pills">
          <span class="pill">AWS</span><span class="pill">Vercel</span><span class="pill">Docker</span><span class="pill">Terraform</span>
        </div>
      </div>
      <div class="stack-row">
        <div class="stack-cat">DevOps</div>
        <div class="stack-pills">
          <span class="pill">GitHub Actions</span><span class="pill">Railway</span><span class="pill">CI/CD</span>
        </div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">03 — Numbers</div>
    <div class="stats-grid">
      <div class="stat-box"><div class="stat-num">50+</div><div class="stat-label">Projects shipped</div></div>
      <div class="stat-box"><div class="stat-num">&lt;2w</div><div class="stat-label">Avg MVP timeline</div></div>
      <div class="stat-box"><div class="stat-num">3</div><div class="stat-label">Core engineers</div></div>
      <div class="stat-box"><div class="stat-num">100%</div><div class="stat-label">Client code ownership</div></div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">04 — Process</div>
    <div style="display:flex; gap:0; align-items:stretch;">
      <div class="process-step" style="border-radius:6px 0 0 6px;">
        <div class="process-num">WEEK 01</div>
        <div class="process-title">Discovery</div>
        <ul class="process-items">
          <li>Scope it</li>
          <li>Price it</li>
          <li>Start fast</li>
        </ul>
      </div>
      <div class="process-step" style="border-radius:0; border-left:none;">
        <div class="process-num">WEEK 02–N</div>
        <div class="process-title">Build</div>
        <ul class="process-items">
          <li>Daily standups</li>
          <li>Async-first</li>
          <li>No bloat</li>
        </ul>
      </div>
      <div class="process-step" style="border-radius:0; border-left:none;">
        <div class="process-num">SHIP</div>
        <div class="process-title">Deploy</div>
        <ul class="process-items">
          <li>Zero-downtime</li>
          <li>CI/CD baked in</li>
          <li>You own the code</li>
        </ul>
      </div>
      <div class="process-step" style="border-radius:0 6px 6px 0; border-left:none; border-right:0.5px solid #1a1a1a;">
        <div class="process-num">POST-LAUNCH</div>
        <div class="process-title">Iterate</div>
        <ul class="process-items">
          <li>Monitor + fix</li>
          <li>We don't disappear</li>
          <li>Scale support</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">05 — Clients say</div>
    <div class="quote-block">
      <div class="quote-text">"Syntaxo built our entire AI automation layer in under three weeks. The quality was unlike anything I'd seen from an agency before."</div>
      <div class="quote-attr">— SAAS FOUNDER, YC W24</div>
    </div>
    <div class="quote-block">
      <div class="quote-text">"They think in systems, not just features. First engineering team that actually understood our scale problem."</div>
      <div class="quote-attr">— CTO, SERIES A STARTUP</div>
    </div>
  </div>

  <div class="cta-block">
    <div class="cta-eyebrow">06 — Let's build</div>
    <div class="cta-headline">Got an idea?<br/>Let's make it real.</div>
    <div class="cta-sub">We take on 2–3 new clients per month. Don't miss the window.</div>
    <div class="cta-buttons">
      <button class="btn-primary" onclick="openLink('https://syntaxo.shvx.dev')">Book a call ↗</button>
      <button class="btn-secondary" onclick="openLink('mailto:hello@syntaxo.tech')">hello@syntaxo.tech</button>
      <button class="btn-secondary" onclick="openLink('https://x.com/syntax_o_tech')">DM on X</button>
    </div>
  </div>

  <div class="footer-line">SYNTAXO © 2025 &nbsp;·&nbsp; SYNTAXO.SHVX.DEV &nbsp;·&nbsp; HELLO@SYNTAXO.TECH</div>

</div>
