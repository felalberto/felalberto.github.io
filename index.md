---
layout: page
title: Home
permalink: /
---

<style>
  .cb-home {
    --cb-primary: #2563eb;
    --cb-primary-dark: #1d4ed8;
    --cb-text: #0f172a;
    --cb-muted: #475569;
    --cb-line: #e2e8f0;
    --cb-soft-blue: #eff6ff;
    --cb-soft-gray: #f8fafc;
    --cb-radius: 20px;
    --cb-shadow: 0 18px 40px rgba(15, 23, 42, 0.08);
    color: var(--cb-text);
  }

  .cb-home * { box-sizing: border-box; }
  .cb-home a { text-decoration: none; }

  .cb-hero {
    display: grid;
    grid-template-columns: minmax(0, 1.25fr) minmax(240px, 0.75fr);
    gap: 26px;
    align-items: center;
    padding: 44px;
    border: 1px solid var(--cb-line);
    border-radius: 28px;
    background: radial-gradient(circle at top right, rgba(37, 99, 235, 0.10), transparent 32%), #ffffff;
    box-shadow: var(--cb-shadow);
    margin-bottom: 34px;
  }

  .cb-eyebrow {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background: var(--cb-soft-blue);
    color: var(--cb-primary-dark);
    border: 1px solid #bfdbfe;
    padding: 7px 12px;
    border-radius: 999px;
    font-size: 0.86rem;
    font-weight: 700;
    margin-bottom: 20px;
  }

  .cb-hero h1 {
    font-size: clamp(2.35rem, 6vw, 4.25rem);
    line-height: 0.96;
    letter-spacing: -0.065em;
    margin: 0 0 20px;
    color: var(--cb-text);
  }

  .cb-lead {
    font-size: 1.13rem;
    color: var(--cb-muted);
    max-width: 700px;
    margin: 0 0 26px;
  }

  .cb-cta-row { display: flex; flex-wrap: wrap; gap: 12px; align-items: center; }

  .cb-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    border-radius: 12px;
    padding: 12px 18px;
    font-weight: 800;
    border: 2px solid var(--cb-primary);
  }

  .cb-button-primary { background: var(--cb-primary); color: #ffffff !important; }
  .cb-button-secondary { background: #ffffff; color: var(--cb-primary) !important; }

  .cb-hero-card {
    background: #0f172a;
    color: #ffffff;
    border-radius: 22px;
    padding: 24px;
    box-shadow: 0 24px 60px rgba(15, 23, 42, 0.20);
  }

  .cb-hero-card h2 { color: #ffffff; margin: 0 0 12px; font-size: 1.18rem; }
  .cb-hero-card p, .cb-hero-card li { color: #dbeafe; }
  .cb-mini-list { display: grid; gap: 10px; margin: 16px 0 0; padding: 0; list-style: none; }

  .cb-audience-strip {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    align-items: center;
    padding: 16px 18px;
    border: 1px solid var(--cb-line);
    border-radius: 18px;
    background: #ffffff;
    box-shadow: 0 8px 22px rgba(15, 23, 42, 0.04);
  }

  .cb-audience-strip strong { color: var(--cb-text); margin-right: 4px; }

  .cb-pill {
    display: inline-flex;
    align-items: center;
    border-radius: 999px;
    padding: 7px 11px;
    background: var(--cb-soft-blue);
    color: var(--cb-primary-dark);
    font-size: 0.88rem;
    font-weight: 700;
  }

  .cb-section { margin-top: 48px; }
  .cb-section-header { margin-bottom: 22px; }

  .cb-kicker {
    color: var(--cb-primary);
    font-weight: 900;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    font-size: 0.78rem;
    margin-bottom: 8px;
  }

  .cb-section h2,
  .cb-final-cta h2 {
    font-size: clamp(1.75rem, 3vw, 2.45rem);
    line-height: 1.05;
    letter-spacing: -0.04em;
    margin: 0 0 10px;
    color: var(--cb-text);
  }

  .cb-section p { color: var(--cb-muted); max-width: 760px; margin: 0; }

  .cb-grid-3 { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 18px; }

  .cb-card {
    background: #ffffff;
    border: 1px solid var(--cb-line);
    border-radius: var(--cb-radius);
    padding: 24px;
    box-shadow: 0 10px 28px rgba(15, 23, 42, 0.05);
  }

  .cb-card h3 { margin: 0 0 8px; font-size: 1.12rem; letter-spacing: -0.02em; color: var(--cb-text); }
  .cb-card p { font-size: 0.96rem; color: var(--cb-muted); margin-bottom: 14px; }

  .cb-icon {
    width: 42px;
    height: 42px;
    border-radius: 12px;
    display: grid;
    place-items: center;
    margin-bottom: 16px;
    font-size: 1.25rem;
    background: var(--cb-soft-blue);
  }

  .cb-resource-list { display: grid; gap: 12px; }
  .cb-resource { display: flex; justify-content: space-between; gap: 20px; align-items: center; background: #ffffff; border: 1px solid var(--cb-line); border-radius: 16px; padding: 18px 20px; color: var(--cb-text) !important; }
  .cb-resource span { color: var(--cb-muted); font-size: 0.95rem; }

  .cb-final-cta {
    text-align: center;
    padding: 50px;
    background: linear-gradient(135deg, #0f172a, #1e3a8a);
    color: #ffffff;
    border-radius: 28px;
    box-shadow: var(--cb-shadow);
  }

  .cb-final-cta h2 { color: #ffffff; }
  .cb-final-cta p { color: #dbeafe; margin: 0 auto 24px; max-width: 720px; }

  .cb-footer { margin-top: 36px; padding-top: 22px; border-top: 1px solid var(--cb-line); color: var(--cb-muted); font-size: 0.95rem; display: flex; flex-wrap: wrap; gap: 16px; justify-content: space-between; }

  @media (max-width: 920px) {
    .cb-hero { grid-template-columns: 1fr; padding: 32px; }
    .cb-grid-3 { grid-template-columns: 1fr; }
  }
</style>

<div class="cb-home">
  <section class="cb-hero">
    <div>
      <div class="cb-eyebrow">Bronx-built • School-ready • AI-era instruction</div>
      <h1>Practical computing education for K–12 schools.</h1>
      <p class="cb-lead">
        CodeBronx helps schools turn AI literacy and computer science from abstract initiatives into classroom-ready instruction.
      </p>
      <div class="cb-cta-row">
        <a class="cb-button cb-button-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Consultation%20Request">📅 Book a Consultation</a>
        <a class="cb-button cb-button-secondary" href="/services/">View Services</a>
      </div>
    </div>

    <div class="cb-hero-card">
      <h2>Built for</h2>
      <ul class="cb-mini-list">
        <li>✓ Practical PD</li>
        <li>✓ AI literacy</li>
        <li>✓ CT integration</li>
        <li>✓ School implementation</li>
      </ul>
    </div>
  </section>

  <div class="cb-audience-strip">
    <strong>Built for:</strong>
    <span class="cb-pill">Principals</span>
    <span class="cb-pill">District Leaders</span>
    <span class="cb-pill">Teachers</span>
    <span class="cb-pill">Youth Programs</span>
  </div>

  <section class="cb-section" id="services">
    <div class="cb-section-header">
      <div class="cb-kicker">What CodeBronx helps schools do</div>
      <h2>Make computing education usable.</h2>
      <p>Start with existing instruction, then build practical connections to computational thinking, AI literacy, and computer science.</p>
    </div>

    <div class="cb-grid-3">
      <div class="cb-card">
        <div class="cb-icon">🧠</div>
        <h3>Integrate CT into instruction</h3>
        <p>Connect decomposition, patterns, abstraction, and algorithms to ELA, Math, STEM, and student problem solving.</p>
        <a class="cb-button cb-button-secondary" href="/services/">Explore services</a>
      </div>

      <div class="cb-card">
        <div class="cb-icon">🤖</div>
        <h3>Build AI literacy</h3>
        <p>Help students think first, use AI responsibly, analyze output, verify claims, and explain decisions.</p>
        <a class="cb-button cb-button-secondary" href="/services/">Explore services</a>
      </div>

      <div class="cb-card">
        <div class="cb-icon">🛠️</div>
        <h3>Support teachers</h3>
        <p>Design professional learning, coaching, and classroom-ready materials that teachers can actually use.</p>
        <a class="cb-button cb-button-secondary" href="/packages/">View packages</a>
      </div>
    </div>
  </section>

  <section class="cb-section" id="next">
    <div class="cb-section-header">
      <div class="cb-kicker">Explore next</div>
      <h2>Go deeper when you are ready.</h2>
      <p>The homepage is the starting point. The deeper pages explain the services, packages, and how to start a conversation.</p>
    </div>

    <div class="cb-resource-list">
      <a class="cb-resource" href="/services/"><div><strong>Services</strong><br><span>See the types of support CodeBronx provides for schools and organizations.</span></div><strong>→</strong></a>
      <a class="cb-resource" href="/packages/"><div><strong>Packages</strong><br><span>Review clear entry points from starter workshops to schoolwide partnerships.</span></div><strong>→</strong></a>
      <a class="cb-resource" href="/contact/"><div><strong>Contact</strong><br><span>Start a conversation about your school, district, or organization’s needs.</span></div><strong>→</strong></a>
    </div>
  </section>

  <section class="cb-section cb-final-cta" id="contact">
    <h2>Ready to build a stronger computing education system?</h2>
    <p>Bring CodeBronx into your school, district, or organization to strengthen instruction, build AI literacy, and make computing education practical.</p>
    <div class="cb-cta-row" style="justify-content:center;">
      <a class="cb-button cb-button-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Consultation%20Request">📅 Book a Consultation</a>
      <a class="cb-button cb-button-secondary" href="/contact/">Contact</a>
    </div>
  </section>

  <div class="cb-footer">
    <div>© CodeBronx / Felix Alberto</div>
    <div><a href="mailto:felalberto@gmail.com">felalberto@gmail.com</a> · <a href="https://www.linkedin.com/in/felix-alberto-78763a36/">LinkedIn</a> · <a href="https://github.com/felalberto">GitHub</a></div>
  </div>
</div>
