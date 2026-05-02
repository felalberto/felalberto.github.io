---
title: About
icon: fas fa-info-circle
order: 3
---

<style>
  .cb-about {
    --cba-primary: #2563eb;
    --cba-primary-dark: #1d4ed8;
    --cba-text: #0f172a;
    --cba-muted: #475569;
    --cba-line: #e2e8f0;
    --cba-soft-blue: #eff6ff;
    --cba-radius: 20px;
    --cba-shadow: 0 18px 40px rgba(15, 23, 42, 0.08);
    color: var(--cba-text);
  }

  .cb-about * { box-sizing: border-box; }
  .cb-about a { text-decoration: none; }

  .cba-hero {
    display: grid;
    grid-template-columns: minmax(0, 1.2fr) minmax(260px, 0.8fr);
    gap: 28px;
    align-items: center;
    padding: 42px;
    border: 1px solid var(--cba-line);
    border-radius: 28px;
    background: radial-gradient(circle at top right, rgba(37, 99, 235, 0.11), transparent 32%), #ffffff;
    box-shadow: var(--cba-shadow);
    margin-bottom: 52px;
  }

  .cba-eyebrow {
    display: inline-flex;
    padding: 7px 12px;
    border-radius: 999px;
    background: var(--cba-soft-blue);
    border: 1px solid #bfdbfe;
    color: var(--cba-primary-dark);
    font-size: 0.86rem;
    font-weight: 700;
    margin-bottom: 18px;
  }

  .cba-hero h1 {
    margin: 0 0 18px;
    font-size: clamp(2.1rem, 5vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.05em;
    color: var(--cba-text);
  }

  .cba-lead {
    font-size: 1.08rem;
    color: var(--cba-muted);
    margin: 0 0 24px;
    max-width: 720px;
  }

  .cba-btn-row { display: flex; flex-wrap: wrap; gap: 12px; }
  .cba-btn { display: inline-flex; align-items: center; justify-content: center; border-radius: 12px; padding: 12px 18px; border: 2px solid var(--cba-primary); font-weight: 800; }
  .cba-btn-primary { background: var(--cba-primary); color: #fff !important; }
  .cba-btn-secondary { background: #fff; color: var(--cba-primary) !important; }

  .cba-card-dark {
    background: #0f172a;
    color: #fff;
    border-radius: 22px;
    padding: 24px;
    box-shadow: 0 24px 60px rgba(15, 23, 42, 0.2);
  }

  .cba-card-dark h2 { color: #fff; margin: 0 0 12px; font-size: 1.2rem; }
  .cba-card-dark p, .cba-card-dark li { color: #dbeafe; }
  .cba-list-clean { list-style: none; padding: 0; margin: 16px 0 0; display: grid; gap: 10px; }

  .cba-section { margin-top: 56px; }
  .cba-section-header { margin-bottom: 22px; }
  .cba-kicker { color: var(--cba-primary); font-weight: 900; text-transform: uppercase; letter-spacing: 0.1em; font-size: 0.78rem; margin-bottom: 8px; }

  .cba-section h2,
  .cba-final-cta h2 {
    margin: 0 0 10px;
    font-size: clamp(1.7rem, 3vw, 2.4rem);
    line-height: 1.06;
    letter-spacing: -0.04em;
    color: var(--cba-text);
  }

  .cba-section p { color: var(--cba-muted); max-width: 820px; margin: 0; }

  .cba-grid { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 18px; }
  .cba-card { background: #fff; border: 1px solid var(--cba-line); border-radius: var(--cba-radius); padding: 26px; box-shadow: 0 10px 28px rgba(15, 23, 42, 0.05); }
  .cba-card h3 { margin: 0 0 8px; font-size: 1.18rem; letter-spacing: -0.03em; color: var(--cba-text); }
  .cba-card p { color: var(--cba-muted); }

  .cba-proof-grid { display: grid; grid-template-columns: repeat(4, minmax(0, 1fr)); gap: 18px; }
  .cba-proof strong { display: block; font-size: 1.7rem; letter-spacing: -0.04em; color: var(--cba-text); margin-bottom: 6px; }

  .cba-final-cta {
    text-align: center;
    padding: 48px;
    background: linear-gradient(135deg, #0f172a, #1e3a8a);
    border-radius: 28px;
    box-shadow: var(--cba-shadow);
  }

  .cba-final-cta h2 { color: #fff; }
  .cba-final-cta p { color: #dbeafe; max-width: 760px; margin: 0 auto 22px; }

  @media (max-width: 920px) {
    .cba-hero, .cba-grid, .cba-proof-grid { grid-template-columns: 1fr; }
    .cba-hero { padding: 30px; }
  }
</style>

<div class="cb-about">
  <section class="cba-hero">
    <div>
      <div class="cba-eyebrow">About CodeBronx</div>
      <h1>Bronx-built computing education for schools preparing students for what comes next.</h1>
      <p class="cba-lead">
        CodeBronx is led by Felix Alberto, a curriculum developer and computing education strategist focused on helping schools integrate computational thinking, AI literacy, computer science, robotics, and teacher-ready instructional systems.
      </p>
      <div class="cba-btn-row">
        <a class="cba-btn cba-btn-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Inquiry">📅 Start a Conversation</a>
        <a class="cba-btn cba-btn-secondary" href="/services/">View Services</a>
      </div>
    </div>

    <div class="cba-card-dark">
      <h2>Core belief</h2>
      <p>Computing education should not be a separate, isolated program. It should strengthen how students read, reason, solve problems, create, and prepare for an AI-driven world.</p>
      <ul class="cba-list-clean">
        <li>✓ Practical over performative</li>
        <li>✓ Teacher-ready over theory-heavy</li>
        <li>✓ Integrated over disconnected</li>
        <li>✓ Equity-centered and implementation-focused</li>
      </ul>
    </div>
  </section>

  <section class="cba-section">
    <div class="cba-section-header">
      <div class="cba-kicker">The work</div>
      <h2>Helping schools make computing education useful.</h2>
      <p>
        CodeBronx works at the intersection of curriculum design, professional development, classroom implementation, AI literacy, and career-connected STEM learning. The goal is to help schools build systems teachers can use and students can experience directly.
      </p>
    </div>

    <div class="cba-grid">
      <div class="cba-card">
        <h3>Instructional Design</h3>
        <p>Designing lessons, tools, slide decks, handouts, and implementation guides that help teachers bring computing concepts into real classroom instruction.</p>
      </div>
      <div class="cba-card">
        <h3>Professional Learning</h3>
        <p>Facilitating practical PD that gives educators classroom-ready strategies instead of abstract technology talk.</p>
      </div>
      <div class="cba-card">
        <h3>Computational Thinking Integration</h3>
        <p>Helping schools connect decomposition, pattern recognition, abstraction, and algorithmic thinking to ELA, Math, STEM, and student problem solving.</p>
      </div>
      <div class="cba-card">
        <h3>AI Literacy and Future Readiness</h3>
        <p>Building student and teacher routines that support thoughtful, responsible, and explainable use of AI tools.</p>
      </div>
    </div>
  </section>

  <section class="cba-section">
    <div class="cba-section-header">
      <div class="cba-kicker">Experience that transfers</div>
      <h2>Built from classroom and school implementation.</h2>
      <p>Felix brings experience across K–12 computer science education, curriculum development, teacher coaching, robotics, professional development, and standards-aligned instructional design.</p>
    </div>

    <div class="cba-proof-grid">
      <div class="cba-card cba-proof"><strong>K–8</strong><p>Teacher-facing PD, coaching, and classroom support.</p></div>
      <div class="cba-card cba-proof"><strong>NYC</strong><p>Experience supporting public school implementation and access-focused computing education.</p></div>
      <div class="cba-card cba-proof"><strong>ELA + Math</strong><p>Computational thinking connected to core academic instruction.</p></div>
      <div class="cba-card cba-proof"><strong>AI + CS</strong><p>Foundational literacy tied to student thinking, tools, and artifacts.</p></div>
    </div>
  </section>

  <section class="cba-section cba-final-cta">
    <h2>Want to build practical computing education at your school?</h2>
    <p>Start with a conversation about your goals, grade bands, timeline, and current instructional priorities.</p>
    <div class="cba-btn-row" style="justify-content:center;">
      <a class="cba-btn cba-btn-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Inquiry">📅 Start a Conversation</a>
      <a class="cba-btn cba-btn-secondary" href="/packages/">View Packages</a>
    </div>
  </section>
</div>
