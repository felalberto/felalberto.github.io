---
title: Contact
icon: fas fa-envelope
order: 4
---

<style>
  .cb-contact {
    --cbc-primary: #2563eb;
    --cbc-primary-dark: #1d4ed8;
    --cbc-text: #0f172a;
    --cbc-muted: #475569;
    --cbc-line: #e2e8f0;
    --cbc-soft-blue: #eff6ff;
    --cbc-radius: 20px;
    --cbc-shadow: 0 18px 40px rgba(15, 23, 42, 0.08);
    color: var(--cbc-text);
  }

  .cb-contact * { box-sizing: border-box; }
  .cb-contact a { text-decoration: none; }

  .cbc-hero {
    display: grid;
    grid-template-columns: minmax(0, 1.2fr) minmax(260px, 0.8fr);
    gap: 28px;
    align-items: center;
    padding: 42px;
    border: 1px solid var(--cbc-line);
    border-radius: 28px;
    background: radial-gradient(circle at top right, rgba(37, 99, 235, 0.11), transparent 32%), #ffffff;
    box-shadow: var(--cbc-shadow);
    margin-bottom: 52px;
  }

  .cbc-eyebrow {
    display: inline-flex;
    padding: 7px 12px;
    border-radius: 999px;
    background: var(--cbc-soft-blue);
    border: 1px solid #bfdbfe;
    color: var(--cbc-primary-dark);
    font-size: 0.86rem;
    font-weight: 700;
    margin-bottom: 18px;
  }

  .cbc-hero h1 {
    margin: 0 0 18px;
    font-size: clamp(2.1rem, 5vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.05em;
    color: var(--cbc-text);
  }

  .cbc-lead { font-size: 1.08rem; color: var(--cbc-muted); margin: 0 0 24px; max-width: 720px; }
  .cbc-btn-row { display: flex; flex-wrap: wrap; gap: 12px; }
  .cbc-btn { display: inline-flex; align-items: center; justify-content: center; border-radius: 12px; padding: 12px 18px; border: 2px solid var(--cbc-primary); font-weight: 800; }
  .cbc-btn-primary { background: var(--cbc-primary); color: #fff !important; }
  .cbc-btn-secondary { background: #fff; color: var(--cbc-primary) !important; }

  .cbc-card-dark { background: #0f172a; color: #fff; border-radius: 22px; padding: 24px; box-shadow: 0 24px 60px rgba(15, 23, 42, 0.2); }
  .cbc-card-dark h2 { color: #fff; margin: 0 0 12px; font-size: 1.2rem; }
  .cbc-card-dark p, .cbc-card-dark li { color: #dbeafe; }
  .cbc-list-clean { list-style: none; padding: 0; margin: 16px 0 0; display: grid; gap: 10px; }

  .cbc-section { margin-top: 56px; }
  .cbc-section-header { margin-bottom: 22px; }
  .cbc-kicker { color: var(--cbc-primary); font-weight: 900; text-transform: uppercase; letter-spacing: 0.1em; font-size: 0.78rem; margin-bottom: 8px; }
  .cbc-section h2 { margin: 0 0 10px; font-size: clamp(1.7rem, 3vw, 2.4rem); line-height: 1.06; letter-spacing: -0.04em; color: var(--cbc-text); }
  .cbc-section p { color: var(--cbc-muted); max-width: 780px; margin: 0; }

  .cbc-grid { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 18px; }
  .cbc-card { background: #fff; border: 1px solid var(--cbc-line); border-radius: var(--cbc-radius); padding: 26px; box-shadow: 0 10px 28px rgba(15, 23, 42, 0.05); }
  .cbc-card h3 { margin: 0 0 8px; font-size: 1.18rem; letter-spacing: -0.03em; color: var(--cbc-text); }
  .cbc-card p { color: var(--cbc-muted); margin-bottom: 14px; }
  .cbc-card ul { color: var(--cbc-muted); margin-bottom: 0; }

  @media (max-width: 920px) {
    .cbc-hero, .cbc-grid { grid-template-columns: 1fr; }
    .cbc-hero { padding: 30px; }
  }
</style>

<div class="cb-contact">
  <section class="cbc-hero">
    <div>
      <div class="cbc-eyebrow">Start a conversation</div>
      <h1>Let’s talk about what your school is trying to build.</h1>
      <p class="cbc-lead">
        Reach out if your school, district, or organization needs support with computational thinking, AI literacy, computer science integration, robotics, professional development, or curriculum design.
      </p>
      <div class="cbc-btn-row">
        <a class="cbc-btn cbc-btn-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Consultation%20Request">📅 Email CodeBronx</a>
        <a class="cbc-btn cbc-btn-secondary" href="/packages/">View Packages</a>
      </div>
    </div>

    <div class="cbc-card-dark">
      <h2>Helpful details to include</h2>
      <p>A strong first message helps scope the right support quickly.</p>
      <ul class="cbc-list-clean">
        <li>✓ School or organization name</li>
        <li>✓ Grade bands or audience</li>
        <li>✓ Topic area: AI, CT, CS, robotics, PD, or curriculum</li>
        <li>✓ Timeline and preferred format</li>
      </ul>
    </div>
  </section>

  <section class="cbc-section">
    <div class="cbc-section-header">
      <div class="cbc-kicker">Contact</div>
      <h2>Ways to connect</h2>
      <p>Use email for now. A formal intake form can be added later once the service menu and packages are fully finalized.</p>
    </div>

    <div class="cbc-grid">
      <div class="cbc-card">
        <h3>Email</h3>
        <p>For consultation requests, workshop inquiries, curriculum support, and school partnership conversations.</p>
        <a class="cbc-btn cbc-btn-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Consultation%20Request">felalberto@gmail.com</a>
      </div>
      <div class="cbc-card">
        <h3>Best-fit requests</h3>
        <ul>
          <li>Professional development for teachers</li>
          <li>AI literacy planning</li>
          <li>Computational thinking integration</li>
          <li>Curriculum or lesson design</li>
          <li>Robotics/STEM implementation support</li>
          <li>Schoolwide or districtwide planning</li>
        </ul>
      </div>
    </div>
  </section>
</div>
