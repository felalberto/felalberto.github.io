---
title: Packages
icon: fas fa-layer-group
order: 2
---

<style>
  .cb-packages {
    --cbp-primary: #2563eb;
    --cbp-primary-dark: #1d4ed8;
    --cbp-text: #0f172a;
    --cbp-muted: #475569;
    --cbp-line: #e2e8f0;
    --cbp-soft-blue: #eff6ff;
    --cbp-soft-gray: #f8fafc;
    --cbp-radius: 20px;
    --cbp-shadow: 0 18px 40px rgba(15, 23, 42, 0.08);
    color: var(--cbp-text);
  }

  .cb-packages * { box-sizing: border-box; }
  .cb-packages a { text-decoration: none; }

  .cbp-hero {
    display: grid;
    grid-template-columns: minmax(0, 1.2fr) minmax(260px, 0.8fr);
    gap: 28px;
    align-items: center;
    padding: 42px;
    border: 1px solid var(--cbp-line);
    border-radius: 28px;
    background: radial-gradient(circle at top right, rgba(37, 99, 235, 0.11), transparent 32%), #ffffff;
    box-shadow: var(--cbp-shadow);
    margin-bottom: 52px;
  }

  .cbp-eyebrow {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 7px 12px;
    border-radius: 999px;
    background: var(--cbp-soft-blue);
    border: 1px solid #bfdbfe;
    color: var(--cbp-primary-dark);
    font-size: 0.86rem;
    font-weight: 700;
    margin-bottom: 18px;
  }

  .cbp-hero h1 {
    margin: 0 0 18px;
    font-size: clamp(2.1rem, 5vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.05em;
    color: var(--cbp-text);
  }

  .cbp-lead {
    font-size: 1.08rem;
    color: var(--cbp-muted);
    margin: 0 0 24px;
    max-width: 720px;
  }

  .cbp-cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
  }

  .cbp-btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    border-radius: 12px;
    padding: 12px 18px;
    border: 2px solid var(--cbp-primary);
    font-weight: 800;
  }

  .cbp-btn-primary {
    background: var(--cbp-primary);
    color: #fff !important;
  }

  .cbp-btn-secondary {
    background: #fff;
    color: var(--cbp-primary) !important;
  }

  .cbp-hero-card {
    background: #0f172a;
    color: #fff;
    border-radius: 22px;
    padding: 24px;
    box-shadow: 0 24px 60px rgba(15, 23, 42, 0.2);
  }

  .cbp-hero-card h2 {
    margin: 0 0 12px;
    color: #fff;
    font-size: 1.2rem;
  }

  .cbp-hero-card p,
  .cbp-hero-card li {
    color: #dbeafe;
  }

  .cbp-mini-list {
    list-style: none;
    padding: 0;
    margin: 16px 0 0;
    display: grid;
    gap: 10px;
  }

  .cbp-section { margin-top: 56px; }
  .cbp-section-header { margin-bottom: 22px; }

  .cbp-kicker {
    color: var(--cbp-primary);
    font-weight: 900;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    font-size: 0.78rem;
    margin-bottom: 8px;
  }

  .cbp-section h2,
  .cbp-final-cta h2,
  .cbp-why h2 {
    margin: 0 0 10px;
    font-size: clamp(1.7rem, 3vw, 2.4rem);
    line-height: 1.06;
    letter-spacing: -0.04em;
    color: var(--cbp-text);
  }

  .cbp-section p {
    color: var(--cbp-muted);
    max-width: 760px;
    margin: 0;
  }

  .cbp-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 18px;
  }

  .cbp-card {
    background: #fff;
    border: 1px solid var(--cbp-line);
    border-radius: var(--cbp-radius);
    padding: 26px;
    box-shadow: 0 10px 28px rgba(15, 23, 42, 0.05);
  }

  .cbp-card-featured {
    border: 2px solid #bfdbfe;
    background: linear-gradient(180deg, #f8fbff 0%, #ffffff 30%);
  }

  .cbp-badge {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 6px 11px;
    border-radius: 999px;
    background: var(--cbp-soft-blue);
    color: var(--cbp-primary-dark);
    font-size: 0.8rem;
    font-weight: 800;
    margin-bottom: 14px;
  }

  .cbp-card h3 {
    margin: 0 0 8px;
    font-size: 1.28rem;
    letter-spacing: -0.03em;
    color: var(--cbp-text);
  }

  .cbp-bestfor {
    color: var(--cbp-primary-dark);
    font-weight: 700;
    margin-bottom: 12px;
    font-size: 0.95rem;
  }

  .cbp-card p {
    color: var(--cbp-muted);
    margin-bottom: 14px;
  }

  .cbp-subtitle {
    margin-top: 16px;
    margin-bottom: 8px;
    font-weight: 800;
    color: var(--cbp-text);
    font-size: 0.96rem;
  }

  .cbp-list {
    margin: 0;
    padding-left: 1.15rem;
    color: var(--cbp-muted);
  }

  .cbp-list li { margin-bottom: 0.35rem; }

  .cbp-compare {
    overflow-x: auto;
    background: #fff;
    border: 1px solid var(--cbp-line);
    border-radius: 18px;
    box-shadow: 0 10px 24px rgba(15, 23, 42, 0.04);
  }

  .cbp-compare table {
    width: 100%;
    border-collapse: collapse;
  }

  .cbp-compare th,
  .cbp-compare td {
    text-align: left;
    padding: 16px 18px;
    border-bottom: 1px solid var(--cbp-line);
    vertical-align: top;
  }

  .cbp-compare th {
    background: var(--cbp-soft-gray);
    color: var(--cbp-text);
    font-weight: 800;
  }

  .cbp-compare tr:last-child td { border-bottom: none; }

  .cbp-why {
    display: grid;
    grid-template-columns: 0.95fr 1.05fr;
    gap: 26px;
    background: #0f172a;
    border-radius: 28px;
    padding: 36px;
    box-shadow: var(--cbp-shadow);
  }

  .cbp-why h2,
  .cbp-why .cbp-kicker { color: #fff; }
  .cbp-why p,
  .cbp-why li { color: #cbd5e1; }

  .cbp-pill-grid {
    display: grid;
    gap: 12px;
  }

  .cbp-pill {
    background: rgba(255,255,255,0.08);
    border: 1px solid rgba(255,255,255,0.12);
    border-radius: 16px;
    padding: 14px 16px;
    color: #fff;
    font-weight: 700;
  }

  .cbp-final-cta {
    text-align: center;
    padding: 48px;
    background: linear-gradient(135deg, #0f172a, #1e3a8a);
    border-radius: 28px;
    box-shadow: var(--cbp-shadow);
  }

  .cbp-final-cta h2 { color: #fff; }

  .cbp-final-cta p {
    color: #dbeafe;
    max-width: 760px;
    margin: 0 auto 22px;
  }

  @media (max-width: 920px) {
    .cbp-hero,
    .cbp-why {
      grid-template-columns: 1fr;
      padding: 30px;
    }
    .cbp-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="cb-packages">
  <section class="cbp-hero">
    <div>
      <div class="cbp-eyebrow">Clear ways to work with CodeBronx</div>
      <h1>Packages built for real school implementation.</h1>
      <p class="cbp-lead">
        These packages give schools and organizations a practical path from awareness to implementation.
        The structure is flexible, but the goal stays the same: build computing education that teachers can actually use.
      </p>
      <div class="cbp-cta-row">
        <a class="cbp-btn cbp-btn-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Package%20Inquiry">📅 Book a Consultation</a>
        <a class="cbp-btn cbp-btn-secondary" href="/services/">View Services</a>
      </div>
    </div>

    <div class="cbp-hero-card">
      <h2>What these packages are designed to do</h2>
      <p>Help schools move from interest to actual implementation without adding another disconnected initiative.</p>
      <ul class="cbp-mini-list">
        <li>✓ Build shared language around CT, AI literacy, and CS integration</li>
        <li>✓ Give teachers usable tools and classroom-ready examples</li>
        <li>✓ Support planning, coaching, and implementation when needed</li>
        <li>✓ Create a path from single workshop to schoolwide support</li>
      </ul>
    </div>
  </section>

  <section class="cbp-section">
    <div class="cbp-section-header">
      <div class="cbp-kicker">Choose the right entry point</div>
      <h2>Four ways to work together.</h2>
      <p>Each package is built for a different level of readiness, from first exposure to long-term implementation and custom design support.</p>
    </div>

    <div class="cbp-grid">
      <div class="cbp-card">
        <div class="cbp-badge">Starter</div>
        <h3>Starter Workshop</h3>
        <div class="cbp-bestfor">Best for: schools or organizations exploring computational thinking, AI literacy, or computer science integration.</div>
        <p>A strong entry point for teams that need shared language, practical examples, and a clear next step.</p>
        <div class="cbp-subtitle">Includes</div>
        <ul class="cbp-list">
          <li>One 60- to 90-minute professional development session</li>
          <li>Practical examples tied to ELA, Math, AI literacy, or STEM</li>
          <li>Teacher-facing planning template</li>
          <li>Resource packet</li>
          <li>Optional leadership debrief</li>
        </ul>
      </div>

      <div class="cbp-card cbp-card-featured">
        <div class="cbp-badge">Most practical next step</div>
        <h3>Implementation Sprint</h3>
        <div class="cbp-bestfor">Best for: schools ready to test computing education in real classrooms.</div>
        <p>Moves beyond a single workshop and helps teachers plan, try, and refine classroom-ready activities.</p>
        <div class="cbp-subtitle">Includes</div>
        <ul class="cbp-list">
          <li>2–4 professional learning sessions</li>
          <li>Curriculum review or lesson selection support</li>
          <li>Teacher planning templates</li>
          <li>Classroom-ready lesson extensions</li>
          <li>Optional model lesson or co-planning session</li>
          <li>Implementation reflection tool</li>
          <li>Final recommendations summary</li>
        </ul>
      </div>

      <div class="cbp-card">
        <div class="cbp-badge">Scale</div>
        <h3>Schoolwide Partnership</h3>
        <div class="cbp-bestfor">Best for: schools or districts building a sustainable computing education system.</div>
        <p>Supports planning, professional development, coaching, implementation, and refinement across a longer timeline.</p>
        <div class="cbp-subtitle">Includes</div>
        <ul class="cbp-list">
          <li>Leadership planning session</li>
          <li>Curriculum and instructional priority review</li>
          <li>Multi-session PD series</li>
          <li>Coaching or office hours</li>
          <li>Model lesson support</li>
          <li>Teacher-facing materials and student-facing tools</li>
          <li>Implementation evidence collection</li>
          <li>Final impact summary and roadmap</li>
        </ul>
      </div>

      <div class="cbp-card">
        <div class="cbp-badge">Build</div>
        <h3>Custom Curriculum or Resource Design</h3>
        <div class="cbp-bestfor">Best for: organizations, schools, or programs that need specific materials built.</div>
        <p>For teams that already know what they need but want high-quality, usable instructional assets.</p>
        <div class="cbp-subtitle">Possible deliverables</div>
        <ul class="cbp-list">
          <li>Lesson plans and slide decks</li>
          <li>Student handouts and teacher guides</li>
          <li>Curriculum maps and PD facilitator guides</li>
          <li>AI literacy workflows and CT activities</li>
          <li>Robotics or physical computing challenges</li>
          <li>Implementation toolkits</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="cbp-section">
    <div class="cbp-section-header">
      <div class="cbp-kicker">Need help choosing?</div>
      <h2>Start with the problem you are trying to solve.</h2>
      <p>If you know what your school needs, the right package usually becomes clear fast.</p>
    </div>

    <div class="cbp-compare">
      <table>
        <thead>
          <tr>
            <th>If you need...</th>
            <th>Start with...</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>A clear introduction for staff</td>
            <td><strong>Starter Workshop</strong></td>
          </tr>
          <tr>
            <td>Teachers to try the work in classrooms</td>
            <td><strong>Implementation Sprint</strong></td>
          </tr>
          <tr>
            <td>A schoolwide or districtwide system</td>
            <td><strong>Schoolwide Partnership</strong></td>
          </tr>
          <tr>
            <td>Materials, lessons, or tools built for your program</td>
            <td><strong>Custom Curriculum or Resource Design</strong></td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>

  <section class="cbp-section cbp-why">
    <div>
      <div class="cbp-kicker">What makes this different</div>
      <h2>Not generic tech activities. Actual instructional support.</h2>
      <p>
        CodeBronx starts with instruction, teacher capacity, and student thinking. The goal is not to add more random technology.
        The goal is to make computing education practical, aligned, and sustainable.
      </p>
    </div>

    <div class="cbp-pill-grid">
      <div class="cbp-pill">Practical for real classrooms</div>
      <div class="cbp-pill">Connected to ELA, Math, STEM, and AI literacy</div>
      <div class="cbp-pill">Usable by teachers, not just specialists</div>
      <div class="cbp-pill">Built to move beyond one workshop</div>
      <div class="cbp-pill">Flexible enough for schools, districts, and youth organizations</div>
    </div>
  </section>

  <section class="cbp-section cbp-final-cta">
    <h2>Not sure which package fits?</h2>
    <p>
      Start with a conversation. The right structure depends on your school goals, grade bands,
      timeline, audience, and implementation capacity.
    </p>
    <div class="cbp-cta-row" style="justify-content:center;">
      <a class="cbp-btn cbp-btn-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Package%20Inquiry">📅 Book a Consultation</a>
      <a class="cbp-btn cbp-btn-secondary" href="/services/">View Services</a>
    </div>
  </section>
</div>
