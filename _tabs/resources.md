---
title: Resources
icon: fas fa-toolbox
order: 4
---

<style>
  .cb-resources {
    --cbr-primary: #2563eb;
    --cbr-text: #0f172a;
    --cbr-muted: #475569;
    --cbr-line: #e2e8f0;
    --cbr-soft: #f8fafc;
    --cbr-soft-blue: #eff6ff;
    --cbr-radius: 20px;
    color: var(--cbr-text);
  }

  .cbr-hero {
    padding: 36px;
    border: 1px solid var(--cbr-line);
    border-radius: 28px;
    background: radial-gradient(circle at top right, rgba(37, 99, 235, 0.12), transparent 35%), #ffffff;
    margin-bottom: 34px;
  }

  .cbr-eyebrow {
    display: inline-flex;
    padding: 7px 12px;
    border-radius: 999px;
    background: var(--cbr-soft-blue);
    border: 1px solid #bfdbfe;
    color: #1d4ed8;
    font-size: 0.86rem;
    font-weight: 800;
    margin-bottom: 16px;
  }

  .cbr-hero h1 {
    margin: 0 0 14px;
    font-size: clamp(2rem, 5vw, 3.5rem);
    line-height: 0.98;
    letter-spacing: -0.05em;
  }

  .cbr-hero p {
    margin: 0;
    color: var(--cbr-muted);
    max-width: 760px;
    font-size: 1.05rem;
  }

  .cbr-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 18px;
  }

  .cbr-card {
    display: block;
    padding: 24px;
    border: 1px solid var(--cbr-line);
    border-radius: var(--cbr-radius);
    background: #ffffff;
    text-decoration: none !important;
    color: var(--cbr-text) !important;
    box-shadow: 0 14px 30px rgba(15, 23, 42, 0.06);
  }

  .cbr-card:hover {
    transform: translateY(-2px);
    border-color: #bfdbfe;
  }

  .cbr-card-label {
    display: inline-flex;
    padding: 5px 10px;
    border-radius: 999px;
    background: #e8f8f1;
    color: #087f5b;
    font-size: 0.78rem;
    font-weight: 900;
    letter-spacing: .04em;
    text-transform: uppercase;
    margin-bottom: 12px;
  }

  .cbr-card h2 {
    margin: 0 0 10px;
    letter-spacing: -0.035em;
  }

  .cbr-card p {
    color: var(--cbr-muted);
    margin: 0 0 16px;
  }

  .cbr-card-link {
    font-weight: 900;
    color: var(--cbr-primary);
  }

  @media (max-width: 800px) {
    .cbr-grid { grid-template-columns: 1fr; }
    .cbr-hero { padding: 24px; }
  }
</style>

<div class="cb-resources">
  <section class="cbr-hero">
    <span class="cbr-eyebrow">Free CodeBronx classroom resources</span>
    <h1>Resources for practical computing education.</h1>
    <p>Classroom-ready tools teachers can use to connect computational thinking, computer science, AI literacy, and academic content.</p>
  </section>

  <section class="cbr-grid">
    <a class="cbr-card" href="/resources/code-the-moment/">
      <span class="cbr-card-label">Digital Storytelling + Scratch</span>
      <h2>Code the Moment</h2>
      <p>A free classroom resource that helps students turn one meaningful scene from a story into a Scratch animation using decomposition, sequencing, dialogue, movement, debugging, and reflection.</p>
      <span class="cbr-card-link">Open resource →</span>
    </a>
  </section>
</div>
