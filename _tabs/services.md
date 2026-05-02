---
title: Services
icon: fas fa-briefcase
order: 1
---

<style>
  .cb-services {
    --cbs-primary: #2563eb;
    --cbs-primary-dark: #1d4ed8;
    --cbs-text: #0f172a;
    --cbs-muted: #475569;
    --cbs-line: #e2e8f0;
    --cbs-soft-blue: #eff6ff;
    --cbs-soft-gray: #f8fafc;
    --cbs-radius: 20px;
    --cbs-shadow: 0 18px 40px rgba(15, 23, 42, 0.08);
    color: var(--cbs-text);
  }

  .cb-services * { box-sizing: border-box; }
  .cb-services a { text-decoration: none; }

  .cbs-hero {
    display: grid;
    grid-template-columns: minmax(0, 1.2fr) minmax(260px, 0.8fr);
    gap: 28px;
    align-items: center;
    padding: 42px;
    border: 1px solid var(--cbs-line);
    border-radius: 28px;
    background: radial-gradient(circle at top right, rgba(37, 99, 235, 0.11), transparent 32%), #ffffff;
    box-shadow: var(--cbs-shadow);
    margin-bottom: 52px;
  }

  .cbs-eyebrow {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 7px 12px;
    border-radius: 999px;
    background: var(--cbs-soft-blue);
    border: 1px solid #bfdbfe;
    color: var(--cbs-primary-dark);
    font-size: 0.86rem;
    font-weight: 700;
    margin-bottom: 18px;
  }

  .cbs-hero h1 {
    margin: 0 0 18px;
    font-size: clamp(2.1rem, 5vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.05em;
    color: var(--cbs-text);
  }

  .cbs-lead {
    font-size: 1.08rem;
    color: var(--cbs-muted);
    margin: 0 0 24px;
    max-width: 720px;
  }

  .cbs-cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
  }

  .cbs-btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    border-radius: 12px;
    padding: 12px 18px;
    border: 2px solid var(--cbs-primary);
    font-weight: 800;
  }

  .cbs-btn-primary { background: var(--cbs-primary); color: #fff !important; }
  .cbs-btn-secondary { background: #fff; color: var(--cbs-primary) !important; }

  .cbs-hero-card {
    background: #0f172a;
    color: #fff;
    border-radius: 22px;
    padding: 24px;
    box-shadow: 0 24px 60px rgba(15, 23, 42, 0.2);
  }

  .cbs-hero-card h2 { margin: 0 0 12px; color: #fff; font-size: 1.2rem; }
  .cbs-hero-card p, .cbs-hero-card li { color: #dbeafe; }
  .cbs-mini-list { list-style: none; padding: 0; margin: 16px 0 0; display: grid; gap: 10px; }

  .cbs-section { margin-top: 56px; }
  .cbs-section-header { margin-bottom: 22px; }

  .cbs-kicker {
    color: var(--cbs-primary);
    font-weight: 900;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    font-size: 0.78rem;
    margin-bottom: 8px;
  }

  .cbs-section h2,
  .cbs-method h2,
  .cbs-final-cta h2 {
    margin: 0 0 10px;
    font-size: clamp(1.7rem, 3vw, 2.4rem);
    line-height: 1.06;
    letter-spacing: -0.04em;
    color: var(--cbs-text);
  }

  .cbs-section p { color: var(--cbs-muted); max-width: 760px; margin: 0; }

  .cbs-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 18px;
  }

  .cbs-card {
    background: #fff;
    border: 1px solid var(--cbs-line);
    border-radius: var(--cbs-radius);
    padding: 26px;
    box-shadow: 0 10px 28px rgba(15, 23, 42, 0.05);
  }

  .cbs-icon {
    width: 42px;
    height: 42px;
    border-radius: 12px;
    display: grid;
    place-items: center;
    margin-bottom: 16px;
    font-size: 1.25rem;
    background: var(--cbs-soft-blue);
  }

  .cbs-card h3 {
    margin: 0 0 8px;
    font-size: 1.22rem;
    letter-spacing: -0.03em;
    color: var(--cbs-text);
  }

  .cbs-card p { color: var(--cbs-muted); margin-bottom: 14px; }
  .cbs-subtitle { margin-top: 16px; margin-bottom: 8px; font-weight: 800; color: var(--cbs-text); font-size: 0.96rem; }
  .cbs-list { margin: 0; padding-left: 1.15rem; color: var(--cbs-muted); }
  .cbs-list li { margin-bottom: 0.35rem; }

  .cbs-method {
    display: grid;
    grid-template-columns: 0.9fr 1.1fr;
    gap: 26px;
    background: #0f172a;
    border-radius: 28px;
    padding: 36px;
    box-shadow: var(--cbs-shadow);
  }

  .cbs-method h2, .cbs-method .cbs-kicker { color: #fff; }
  .cbs-method p, .cbs-method span { color: #cbd5e1; }

  .cbs-step-list { display: grid; gap: 12px; }
  .cbs-step { display: grid; grid-template-columns: 40px 1fr; gap: 12px; background: rgba(255,255,255,0.08); border: 1px solid rgba(255,255,255,0.12); border-radius: 16px; padding: 14px 16px; }
  .cbs-step-num { width: 32px; height: 32px; border-radius: 10px; background: #fff; color: #0f172a; display: grid; place-items: center; font-weight: 900; }
  .cbs-step strong { display: block; color: #fff; margin-bottom: 2px; }

  .cbs-final-cta {
    text-align: center;
    padding: 48px;
    background: linear-gradient(135deg, #0f172a, #1e3a8a);
    border-radius: 28px;
    box-shadow: var(--cbs-shadow);
  }

  .cbs-final-cta h2 { color: #fff; }
  .cbs-final-cta p { color: #dbeafe; max-width: 760px; margin: 0 auto 22px; }

  @media (max-width: 920px) {
    .cbs-hero, .cbs-method { grid-template-columns: 1fr; padding: 30px; }
    .cbs-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="cb-services">
  <section class="cbs-hero">
    <div>
      <div class="cbs-eyebrow">Services for schools, districts, and youth programs</div>
      <h1>Computing education that actually fits the classroom.</h1>
      <p class="cbs-lead">
        CodeBronx helps schools integrate computational thinking, AI literacy, and computer science into everyday instruction through practical professional development, coaching, and curriculum support.
      </p>
      <div class="cbs-cta-row">
        <a class="cbs-btn cbs-btn-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Services%20Inquiry">📅 Book a Consultation</a>
        <a class="cbs-btn cbs-btn-secondary" href="/packages/">View Packages</a>
      </div>
    </div>

    <div class="cbs-hero-card">
      <h2>What this work is built for</h2>
      <p>Practical implementation, not one-off tech activities.</p>
      <ul class="cbs-mini-list">
        <li>✓ Teacher-ready lesson materials</li>
        <li>✓ Professional development that leads to classroom use</li>
        <li>✓ AI literacy grounded in student thinking</li>
        <li>✓ Support that can scale beyond one teacher</li>
      </ul>
    </div>
  </section>

  <section class="cbs-section">
    <div class="cbs-section-header">
      <div class="cbs-kicker">What CodeBronx helps schools build</div>
      <h2>Services designed around instruction, not hype.</h2>
      <p>The strongest computing education work starts with real curriculum, real teachers, and real classroom constraints.</p>
    </div>

    <div class="cbs-grid">
      <div class="cbs-card">
        <div class="cbs-icon">🧠</div>
        <h3>Computational Thinking Integration</h3>
        <p>Support for embedding decomposition, pattern recognition, abstraction, and algorithmic thinking into ELA, Math, STEM, and project-based learning.</p>
        <div class="cbs-subtitle">Can include</div>
        <ul class="cbs-list">
          <li>ELA and Math lesson extensions</li>
          <li>Teacher planning templates</li>
          <li>Student graphic organizers and checklists</li>
          <li>Curriculum review to identify natural fit points</li>
        </ul>
      </div>

      <div class="cbs-card">
        <div class="cbs-icon">🤖</div>
        <h3>AI Literacy for Schools</h3>
        <p>Responsible, age-appropriate AI literacy support that helps students think first, analyze output, verify claims, and justify decisions.</p>
        <div class="cbs-subtitle">Can include</div>
        <ul class="cbs-list">
          <li>Student AI literacy routines</li>
          <li>Teacher planning workflows</li>
          <li>Reflection and verification protocols</li>
          <li>School-facing AI guidance</li>
        </ul>
      </div>

      <div class="cbs-card">
        <div class="cbs-icon">🛠️</div>
        <h3>Professional Development</h3>
        <p>Interactive professional learning that gives educators concrete strategies, examples, and materials they can use immediately.</p>
        <div class="cbs-subtitle">Formats</div>
        <ul class="cbs-list">
          <li>60-minute introductory sessions</li>
          <li>90-minute interactive workshops</li>
          <li>Half-day or full-day PD</li>
          <li>Multi-session PD series</li>
        </ul>
      </div>

      <div class="cbs-card">
        <div class="cbs-icon">📈</div>
        <h3>Coaching and Classroom Implementation</h3>
        <p>Support after the PD ends, so teachers can plan, try, reflect, and refine the work in real classrooms.</p>
        <div class="cbs-subtitle">Can include</div>
        <ul class="cbs-list">
          <li>Co-planning with teachers</li>
          <li>Model lesson support</li>
          <li>Classroom implementation feedback</li>
          <li>Student work review</li>
        </ul>
      </div>

      <div class="cbs-card">
        <div class="cbs-icon">⚙️</div>
        <h3>STEM, Robotics, and Physical Computing</h3>
        <p>Hands-on computing experiences through robotics, devices, design challenges, physical computing, and student presentation work.</p>
        <div class="cbs-subtitle">Can include</div>
        <ul class="cbs-list">
          <li>Robotics curriculum planning</li>
          <li>Physical computing activities</li>
          <li>Student design challenges</li>
          <li>Showcase and presentation support</li>
        </ul>
      </div>

      <div class="cbs-card">
        <div class="cbs-icon">📚</div>
        <h3>Custom Curriculum and Resource Design</h3>
        <p>Reusable instructional materials for schools, programs, grants, pilots, and professional learning initiatives.</p>
        <div class="cbs-subtitle">Can include</div>
        <ul class="cbs-list">
          <li>Lesson plans and slide decks</li>
          <li>Student handouts and teacher guides</li>
          <li>Implementation toolkits</li>
          <li>PD facilitator materials</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="cbs-section cbs-method">
    <div>
      <div class="cbs-kicker">The CodeBronx approach</div>
      <h2>Start with the school’s real instructional priorities.</h2>
      <p>CodeBronx does not treat computing as an add-on. The work begins with what schools already teach and builds practical computing connections from there.</p>
    </div>
    <div class="cbs-step-list">
      <div class="cbs-step"><div class="cbs-step-num">1</div><div><strong>Study the current curriculum</strong><span>Identify where computing naturally strengthens existing instruction.</span></div></div>
      <div class="cbs-step"><div class="cbs-step-num">2</div><div><strong>Build teacher-facing tools</strong><span>Create resources teachers can actually use within their current schedules.</span></div></div>
      <div class="cbs-step"><div class="cbs-step-num">3</div><div><strong>Support implementation</strong><span>Use PD, coaching, modeling, and feedback cycles to move from idea to classroom practice.</span></div></div>
      <div class="cbs-step"><div class="cbs-step-num">4</div><div><strong>Refine from evidence</strong><span>Use teacher feedback, student work, and implementation notes to improve the system.</span></div></div>
    </div>
  </section>

  <section class="cbs-section cbs-final-cta">
    <h2>Need help choosing the right service?</h2>
    <p>Start with a conversation. The right structure depends on your goals, timeline, grade band, and implementation capacity.</p>
    <div class="cbs-cta-row" style="justify-content:center;">
      <a class="cbs-btn cbs-btn-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Services%20Inquiry">📅 Book a Consultation</a>
      <a class="cbs-btn cbs-btn-secondary" href="/packages/">View Packages</a>
    </div>
  </section>
</div>
