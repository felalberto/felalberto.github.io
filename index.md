---
layout: page
title: Work
permalink: /
---

<style>
  .cb-work-home {
    --cb-bg: #f4f1ea;
    --cb-paper: #fffdf8;
    --cb-text: #171717;
    --cb-muted: #6f6a62;
    --cb-line: #d8d2c7;
    --cb-dark: #171717;
    --cb-accent: #d64b2a;
    color: var(--cb-text);
    width: min(1180px, calc(100vw - 48px));
    margin: 0 auto;
  }

  .cb-work-home * { box-sizing: border-box; }

  .cb-work-home a {
    text-decoration: none !important;
    color: inherit;
  }

  #breadcrumb,
  .breadcrumb,
  .breadcrumb-wrapper,
  .page-title,
  .post-title,
  .dynamic-title,
  h1.dynamic-title,
  #page-title,
  #panel-wrapper,
  #access-lastmod,
  #access-tags {
    display: none !important;
  }

  @media (min-width: 1200px) {
    #core-wrapper,
    #main-wrapper,
    main,
    .main,
    .main-content,
    #post-wrapper,
    .content,
    article,
    .post-content {
      max-width: none !important;
      width: auto !important;
    }
  }

  .cb-intro {
    padding: 72px 0 58px;
    border-bottom: 1px solid var(--cb-line);
  }

  .cb-kicker {
    margin: 0 0 18px;
    color: var(--cb-muted);
    font-size: .76rem;
    font-weight: 800;
    letter-spacing: .12em;
    text-transform: uppercase;
  }

  .cb-intro h1 {
    max-width: 980px;
    margin: 0;
    color: var(--cb-text);
    font-size: clamp(3rem, 7.5vw, 7.2rem);
    font-weight: 700;
    letter-spacing: -.065em;
    line-height: .92;
  }

  .cb-intro-copy {
    max-width: 700px;
    margin: 34px 0 0;
    color: var(--cb-muted);
    font-size: clamp(1.05rem, 1.7vw, 1.35rem);
    line-height: 1.65;
  }

  .cb-section {
    padding: 64px 0 82px;
  }

  .cb-section-head {
    display: flex;
    align-items: end;
    justify-content: space-between;
    gap: 24px;
    margin-bottom: 28px;
  }

  .cb-section-head h2 {
    margin: 0;
    color: var(--cb-text);
    font-size: clamp(2rem, 4vw, 3.4rem);
    letter-spacing: -.05em;
  }

  .cb-archive-link {
    color: var(--cb-muted) !important;
    font-size: .95rem;
    border-bottom: 1px solid var(--cb-muted);
    padding-bottom: 2px;
  }

  .cb-project-grid {
    display: grid;
    grid-template-columns: repeat(12, minmax(0, 1fr));
    gap: 18px;
  }

  .cb-project-card {
    grid-column: span 6;
    display: flex;
    flex-direction: column;
    min-height: 330px;
    padding: 28px;
    border: 1px solid var(--cb-line);
    background: var(--cb-paper);
    transition: transform .18s ease, border-color .18s ease;
  }

  .cb-project-card:hover {
    transform: translateY(-3px);
    border-color: #a9a095;
  }

  .cb-project-card.cb-featured {
    grid-column: span 12;
    min-height: 430px;
    padding: clamp(30px, 5vw, 54px);
    background: var(--cb-dark);
    color: #fff;
  }

  .cb-card-top {
    display: flex;
    justify-content: space-between;
    gap: 20px;
    align-items: baseline;
    margin-bottom: 54px;
  }

  .cb-project-card.cb-featured .cb-card-top {
    margin-bottom: 92px;
  }

  .cb-project-number,
  .cb-project-date {
    color: var(--cb-muted);
    font-size: .74rem;
    font-weight: 800;
    letter-spacing: .08em;
    text-transform: uppercase;
  }

  .cb-featured .cb-project-number,
  .cb-featured .cb-project-date {
    color: #aaa49c;
  }

  .cb-project-title {
    max-width: 760px;
    margin: 0;
    color: var(--cb-text);
    font-size: clamp(1.55rem, 2.5vw, 2.5rem);
    letter-spacing: -.045em;
    line-height: 1.05;
  }

  .cb-featured .cb-project-title {
    color: #fff;
    font-size: clamp(2.35rem, 5vw, 5rem);
    line-height: .98;
  }

  .cb-project-excerpt {
    max-width: 700px;
    margin: 18px 0 0;
    color: var(--cb-muted);
    font-size: .98rem;
    line-height: 1.65;
  }

  .cb-featured .cb-project-excerpt {
    color: #d2cec8;
    font-size: 1.08rem;
  }

  .cb-card-bottom {
    margin-top: auto;
    padding-top: 32px;
  }

  .cb-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 7px 14px;
  }

  .cb-tags span {
    color: var(--cb-muted);
    font-size: .73rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: .04em;
  }

  .cb-featured .cb-tags span {
    color: #aaa49c;
  }

  .cb-project-image {
    width: 100%;
    aspect-ratio: 16 / 9;
    object-fit: cover;
    margin: -28px -28px 26px;
    width: calc(100% + 56px);
    max-width: none;
  }

  .cb-featured .cb-project-image {
    margin: -54px -54px 34px;
    width: calc(100% + 108px);
  }

  .cb-statement {
    padding: 86px 0;
    border-top: 1px solid var(--cb-line);
  }

  .cb-statement-grid {
    display: grid;
    grid-template-columns: minmax(0, .55fr) minmax(0, 1.45fr);
    gap: 40px;
  }

  .cb-statement-label {
    color: var(--cb-muted);
    font-size: .76rem;
    font-weight: 800;
    letter-spacing: .12em;
    text-transform: uppercase;
  }

  .cb-statement p {
    margin: 0;
    color: var(--cb-text);
    font-size: clamp(1.7rem, 3.4vw, 3.35rem);
    line-height: 1.08;
    letter-spacing: -.045em;
  }

  .cb-collab {
    margin: 0 0 54px;
    padding: clamp(34px, 6vw, 64px);
    background: var(--cb-accent);
    color: #111;
  }

  .cb-collab .cb-kicker {
    color: rgba(0,0,0,.6);
  }

  .cb-collab h2 {
    max-width: 860px;
    margin: 0;
    color: #111;
    font-size: clamp(2.25rem, 5vw, 5rem);
    line-height: .98;
    letter-spacing: -.055em;
  }

  .cb-collab p {
    max-width: 620px;
    margin: 26px 0 0;
    color: rgba(0,0,0,.72);
    font-size: 1.03rem;
    line-height: 1.65;
  }

  .cb-collab-link {
    display: inline-block;
    margin-top: 30px;
    padding-bottom: 3px;
    border-bottom: 2px solid #111;
    color: #111 !important;
    font-weight: 800;
  }

  .cb-note {
    padding: 0 0 56px;
    color: var(--cb-muted);
    font-size: .85rem;
  }

  @media (max-width: 820px) {
    .cb-work-home {
      width: min(100% - 28px, 1180px);
    }

    .cb-intro {
      padding-top: 48px;
    }

    .cb-section-head {
      align-items: flex-start;
      flex-direction: column;
    }

    .cb-project-card,
    .cb-project-card.cb-featured {
      grid-column: span 12;
    }

    .cb-project-card {
      min-height: 280px;
    }

    .cb-project-card.cb-featured {
      min-height: 360px;
      padding: 30px;
    }

    .cb-featured .cb-project-image {
      margin: -30px -30px 28px;
      width: calc(100% + 60px);
    }

    .cb-project-card.cb-featured .cb-card-top {
      margin-bottom: 58px;
    }

    .cb-statement-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="cb-work-home">

  <section class="cb-intro">
    <p class="cb-kicker">CodeBronx / Work in learning + technology</p>
    <h1>Projects before pitches.</h1>
    <p class="cb-intro-copy">
      CodeBronx is a record of work across computing, STEM, AI, curriculum, physical computing,
      teacher learning, and student-centered design. The focus here is the work itself: what was
      built, what learners did, and what came from it.
    </p>
  </section>

  <section class="cb-section">
    <div class="cb-section-head">
      <h2>Selected Work</h2>
      <a class="cb-archive-link" href="/categories/portfolio/">View full portfolio</a>
    </div>

    <div class="cb-project-grid">
      {% assign portfolio = site.categories.Portfolio %}
      {% for post in portfolio limit: 7 %}
        <a class="cb-project-card {% if forloop.first %}cb-featured{% endif %}" href="{{ post.url | relative_url }}">

          {% if post.image %}
            <img class="cb-project-image" src="{{ post.image | relative_url }}" alt="">
          {% endif %}

          <div class="cb-card-top">
            <span class="cb-project-number">Project {{ forloop.index | prepend: '0' }}</span>
            <span class="cb-project-date">{{ post.date | date: "%Y" }}</span>
          </div>

          <div>
            <h3 class="cb-project-title">{{ post.title }}</h3>

            <p class="cb-project-excerpt">
              {% if post.description %}
                {{ post.description }}
              {% elsif post.excerpt %}
                {{ post.excerpt | strip_html | strip_newlines | truncate: 220 }}
              {% else %}
                Open the project to explore the work, process, and artifacts.
              {% endif %}
            </p>
          </div>

          {% if post.tags %}
            <div class="cb-card-bottom">
              <div class="cb-tags">
                {% for tag in post.tags limit: 4 %}
                  <span>{{ tag }}</span>
                {% endfor %}
              </div>
            </div>
          {% endif %}
        </a>
      {% endfor %}
    </div>
  </section>

  <section class="cb-statement">
    <div class="cb-statement-grid">
      <div class="cb-statement-label">What connects the work</div>
      <p>
        Technology matters most when learners use it to investigate, make, test, explain, and respond
        to something that matters.
      </p>
    </div>
  </section>

  <section class="cb-collab">
    <p class="cb-kicker">Collaborate</p>
    <h2>Building something that overlaps with this work?</h2>
    <p>
      CodeBronx occasionally collaborates with schools, universities, community organizations,
      and education teams on curriculum, learning design, emerging technology, and youth-centered STEM work.
    </p>
    <a class="cb-collab-link" href="mailto:felalberto@gmail.com?subject=CodeBronx%20Collaboration">Start a conversation →</a>
  </section>

  <div class="cb-note">
    Project photography and artifacts will be added from original CodeBronx and partner work only.
  </div>

</div>
