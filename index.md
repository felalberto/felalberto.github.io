---
layout: page
title: Home
permalink: /
---

<style>
  .cb-home {
    --cb-bg: #f8fafc;
    --cb-panel: #ffffff;
    --cb-text: #0f172a;
    --cb-muted: #475569;
    --cb-line: #e2e8f0;
    --cb-primary: #2563eb;
    --cb-primary-dark: #1d4ed8;
    --cb-soft-blue: #eff6ff;
    --cb-radius: 18px;
    --cb-shadow: 0 20px 45px rgba(15, 23, 42, 0.08);
    color: var(--cb-text);
  }

  .cb-home * {
    box-sizing: border-box;
  }

  .cb-home a {
    text-decoration: none;
  }

  .cb-hero {
    display: grid;
    grid-template-columns: minmax(0, 1.25fr) minmax(280px, 0.75fr);
    gap: 32px;
    align-items: center;
    padding: 46px;
    background: radial-gradient(circle at top right, rgba(37, 99, 235, 0.14), transparent 34%), var(--cb-panel);
    border: 1px solid var(--cb-line);
    border-radius: 28px;
    box-shadow: var(--cb-shadow);
    overflow: hidden;
    margin-bottom: 54px;
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
    margin-bottom: 22px;
  }

  .cb-hero h1 {
    font-size: clamp(2.35rem, 6vw, 4.25rem);
    line-height: 0.96;
    letter-spacing: -0.065em;
    margin: 0 0 22px;
    color: var(--cb-text);
  }

  .cb-lead {
    font-size: 1.15rem;
    color: var(--cb-muted);
    max-width: 720px;
    margin: 0 0 30px;
  }

  .cb-cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    align-items: center;
  }

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

  .cb-button-primary {
    background: var(--cb-primary);
    color: #ffffff !important;
  }

  .cb-button-secondary {
    background: #ffffff;
    color: var(--cb-primary) !important;
  }

  .cb-hero-card {
    background: #0f172a;
    color: #ffffff;
    border-radius: 22px;
    padding: 26px;
    box-shadow: 0 24px 60px rgba(15, 23, 42, 0.22);
  }

  .cb-hero-card h2 {
    color: #ffffff;
    margin: 0 0 14px;
    font-size: 1.25rem;
  }

  .cb-hero-card p {
    color: #dbeafe;
    margin-bottom: 16px;
  }

  .cb-mini-list {
    display: grid;
    gap: 12px;
    margin: 18px 0 0;
    padding: 0;
    list-style: none;
  }

  .cb-mini-list li {
    color: #dbeafe;
    font-size: 0.95rem;
  }

  .cb-section {
    margin-top: 58px;
  }

  .cb-section-header {
    margin-bottom: 24px;
  }

  .cb-kicker {
    color: var(--cb-primary);
    font-weight: 900;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    font-size: 0.78rem;
    margin-bottom: 8px;
  }

  .cb-section h2,
  .cb-method h2,
  .cb-final-cta h2 {
    font-size: clamp(1.8rem, 3vw, 2.55rem);
    line-height: 1.05;
    letter-spacing: -0.04em;
    margin: 0 0 10px;
    color: var(--cb-text);
  }

  .cb-section p {
    color: var(--cb-muted);
    max-width: 760px;
    margin: 0;
  }

  .cb-audience-grid,
  .cb-offer-grid,
  .cb-proof-grid {
    display: grid;
    gap: 18px;
  }

  .cb-audience-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }

  .cb-offer-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .cb-proof-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
  }

  .cb-card {
    background: var(--cb-panel);
    border: 1px solid var(--cb-line);
    border-radius: var(--cb-radius);
    padding: 24px;
    box-shadow: 0 10px 28px rgba(15, 23, 42, 0.05);
  }

  .cb-card h3 {
    margin: 0 0 8px;
    font-size: 1.1rem;
    letter-spacing: -0.02em;
    color: var(--cb-text);
  }

  .cb-card p {
    font-size: 0.96rem;
    color: var(--cb-muted);
  }

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

  .cb-method {
    background: var(--cb-text);
    color: #ffffff;
    border-radius: 28px;
    padding: 38px;
    display: grid;
    grid-template-columns: 0.85fr 1.15fr;
    gap: 28px;
    align-items: start;
    box-shadow: var(--cb-shadow);
  }

  .cb-method h2,
  .cb-method .cb-kicker {
    color: #ffffff;
  }

  .cb-method p {
    color: #cbd5e1;
  }

  .cb-steps {
    display: grid;
    gap: 12px;
  }

  .cb-step {
    background: rgba(255,255,255,0.08);
    border: 1px solid rgba(255,255,255,0.14);
    border-radius: 16px;
    padding: 16px;
    display: grid;
    grid-template-columns: 42px 1fr;
    gap: 12px;
  }

  .cb-step-number {
    width: 34px;
    height: 34px;
    border-radius: 10px;
    background: #ffffff;
    color: var(--cb-text);
    display: grid;
    place-items: center;
    font-weight: 900;
  }

  .cb-step strong {
    display: block;
    margin-bottom: 3px;
    color: #ffffff;
  }

  .cb-step span {
    color: #cbd5e1;
    font-size: 0.92rem;
  }

  .cb-proof-card strong {
    display: block;
    font-size: 1.9rem;
    letter-spacing: -0.04em;
    margin-bottom: 6px;
    color: var(--cb-text);
  }

  .cb-resource-list {
    display: grid;
    gap: 12px;
  }

  .cb-resource {
    display: flex;
    justify-content: space-between;
    gap: 20px;
    align-items: center;
    background: var(--cb-panel);
    border: 1px solid var(--cb-line);
    border-radius: 16px;
    padding: 18px 20px;
    color: var(--cb-text) !important;
  }

  .cb-resource span {
    color: var(--cb-muted);
    font-size: 0.95rem;
  }

  .cb-final-cta {
    text-align: center;
    padding: 54px;
    background: linear-gradient(135deg, #0f172a, #1e3a8a);
    color: #ffffff;
    border-radius: 28px;
    box-shadow: var(--cb-shadow);
  }

  .cb-final-cta h2 {
    color: #ffffff;
  }

  .cb-final-cta p {
    color: #dbeafe;
    margin: 0 auto 24px;
    max-width: 760px;
  }

  .cb-footer {
    margin-top: 40px;
    padding-top: 24px;
    border-top: 1px solid var(--cb-line);
    color: var(--cb-muted);
    font-size: 0.95rem;
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    justify-content: space-between;
  }

  @media (max-width: 920px) {
    .cb-hero,
    .cb-method {
      grid-template-columns: 1fr;
      padding: 32px;
    }

    .cb-audience-grid,
    .cb-offer-grid,
    .cb-proof-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="cb-home">
  <section class="cb-hero">
    <div>
      <div class="cb-eyebrow">Bronx-built • School-ready • AI-era instruction</div>
      <h1>Practical computing education for K–12 schools.</h1>
      <p class="cb-lead">
        CodeBronx helps schools prepare students for an AI-driven world by integrating computational thinking,
        AI literacy, and computer science into everyday instruction — without adding another disconnected program.
      </p>
      <div class="cb-cta-row">
        <a class="cb-button cb-button-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Consultation%20Request">📅 Book a Consultation</a>
        <a class="cb-button cb-button-secondary" href="#services">View Services</a>
      </div>
    </div>

    <div class="cb-hero-card">
      <h2>What schools get</h2>
      <p>Teacher-facing systems that connect ELA, Math, technology, and career-connected learning.</p>
      <ul class="cb-mini-list">
        <li>✓ Lesson extensions that fit existing curriculum</li>
        <li>✓ Professional development teachers can use immediately</li>
        <li>✓ AI literacy routines students can explain and defend</li>
        <li>✓ Implementation support beyond one-off workshops</li>
      </ul>
    </div>
  </section>

  <section class="cb-section" id="audience">
    <div class="cb-section-header">
      <div class="cb-kicker">Built for real school constraints</div>
      <h2>For leaders who need more than another “tech activity.”</h2>
      <p>
        The goal is not to add more noise to the school day. The goal is to make computing education useful,
        visible, and connected to what students are already learning.
      </p>
    </div>

    <div class="cb-audience-grid">
      <div class="cb-card">
        <div class="cb-icon">🏫</div>
        <h3>For Principals</h3>
        <p>Strengthen instruction with computing education while protecting teacher time and core academic priorities.</p>
      </div>
      <div class="cb-card">
        <div class="cb-icon">🧭</div>
        <h3>For District Leaders</h3>
        <p>Build scalable CS and AI literacy systems that can move beyond a single classroom or one enthusiastic teacher.</p>
      </div>
      <div class="cb-card">
        <div class="cb-icon">👩🏽‍🏫</div>
        <h3>For Teachers</h3>
        <p>Use classroom-ready routines, prompts, and lesson extensions that make computational thinking concrete.</p>
      </div>
    </div>
  </section>

  <section class="cb-section" id="services">
    <div class="cb-section-header">
      <div class="cb-kicker">What I help schools build</div>
      <h2>Computing education that actually fits the classroom.</h2>
      <p>
        CodeBronx focuses on practical implementation: lesson design, teacher learning, student artifacts,
        and systems that can be repeated.
      </p>
    </div>

    <div class="cb-offer-grid">
      <div class="cb-card">
        <div class="cb-icon">🧠</div>
        <h3>Computational Thinking Integration</h3>
        <p>ELA and Math lesson extensions built around decomposition, pattern recognition, abstraction, and algorithmic thinking.</p>
      </div>
      <div class="cb-card">
        <div class="cb-icon">🤖</div>
        <h3>AI Literacy Foundations</h3>
        <p>Age-appropriate routines that help students think first, use AI responsibly, analyze output, and justify decisions.</p>
      </div>
      <div class="cb-card">
        <div class="cb-icon">🛠️</div>
        <h3>Teacher Professional Learning</h3>
        <p>PD and coaching that gives teachers usable strategies, not theory-heavy sessions that disappear after the workshop.</p>
      </div>
      <div class="cb-card">
        <div class="cb-icon">📈</div>
        <h3>Schoolwide Implementation</h3>
        <p>Planning support, resource development, and implementation routines that make CS and AI literacy sustainable.</p>
      </div>
    </div>
  </section>

  <section class="cb-section cb-method" id="method">
    <div>
      <div class="cb-kicker">The CodeBronx method</div>
      <h2>Start with what schools already teach. Build from there.</h2>
      <p>
        The strongest computing education work does not live as a side project. It connects to real curriculum,
        real teachers, and real student thinking.
      </p>
    </div>

    <div class="cb-steps">
      <div class="cb-step">
        <div class="cb-step-number">1</div>
        <div><strong>Study the current curriculum</strong><span>Identify where computing naturally strengthens ELA, Math, STEM, or pathways work.</span></div>
      </div>
      <div class="cb-step">
        <div class="cb-step-number">2</div>
        <div><strong>Design classroom-ready extensions</strong><span>Create short, usable lessons that fit within existing instructional time.</span></div>
      </div>
      <div class="cb-step">
        <div class="cb-step-number">3</div>
        <div><strong>Support teacher implementation</strong><span>Use PD, modeling, coaching, and feedback cycles to move from plan to classroom practice.</span></div>
      </div>
      <div class="cb-step">
        <div class="cb-step-number">4</div>
        <div><strong>Collect evidence and refine</strong><span>Look at student work, teacher feedback, and implementation data to improve the system.</span></div>
      </div>
    </div>
  </section>

  <section class="cb-section" id="proof">
    <div class="cb-section-header">
      <div class="cb-kicker">Experience that transfers</div>
      <h2>Built from NYC school implementation, not theory.</h2>
      <p>
        Felix Alberto brings experience across curriculum design, professional development, classroom coaching,
        robotics, AI literacy, and computational thinking integration.
      </p>
    </div>

    <div class="cb-proof-grid">
      <div class="cb-card cb-proof-card">
        <strong>K–8</strong>
        <p>Teacher-facing professional learning and classroom support.</p>
      </div>
      <div class="cb-card cb-proof-card">
        <strong>NYC</strong>
        <p>Experience supporting public school implementation and equity-focused computing access.</p>
      </div>
      <div class="cb-card cb-proof-card">
        <strong>ELA + Math</strong>
        <p>Computational thinking integrated into core academic instruction.</p>
      </div>
      <div class="cb-card cb-proof-card">
        <strong>AI + CS</strong>
        <p>Foundational literacy connected to real student thinking and artifacts.</p>
      </div>
    </div>
  </section>

  <section class="cb-section" id="resources">
    <div class="cb-section-header">
      <div class="cb-kicker">Resources</div>
      <h2>Tools for educators and school teams.</h2>
      <p>Start with practical resources that help teachers plan, question, revise, and build stronger instruction.</p>
    </div>

    <div class="cb-resource-list">
      <a class="cb-resource" href="https://felalberto.github.io/posts/ct-ai-workflow/">
        <div>
          <strong>Computational Thinking + AI Workflow</strong><br>
          <span>A practical thinking routine for using AI with more structure and judgment.</span>
        </div>
        <strong>→</strong>
      </a>
      <a class="cb-resource" href="#">
        <div>
          <strong>Integrating Computational Thinking Into Instruction</strong><br>
          <span>Placeholder resource page for school-facing CT integration guidance.</span>
        </div>
        <strong>→</strong>
      </a>
      <a class="cb-resource" href="#">
        <div>
          <strong>Teacher Planning With AI</strong><br>
          <span>Placeholder resource page for responsible teacher planning workflows.</span>
        </div>
        <strong>→</strong>
      </a>
    </div>
  </section>

  <section class="cb-section cb-final-cta" id="contact">
    <h2>Ready to build a stronger computing education system?</h2>
    <p>
      Bring CodeBronx into your school, district, or organization to strengthen instruction,
      build AI literacy, and make computing education practical.
    </p>
    <a class="cb-button cb-button-primary" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Consultation%20Request">📅 Book a Consultation</a>
  </section>

  <div class="cb-footer">
    <div>© CodeBronx / Felix Alberto</div>
    <div>
      <a href="mailto:felalberto@gmail.com">felalberto@gmail.com</a> ·
      <a href="https://www.linkedin.com/in/felix-alberto-78763a36/">LinkedIn</a> ·
      <a href="https://github.com/felalberto">GitHub</a>
    </div>
  </div>
</div>
