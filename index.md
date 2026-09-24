---
layout: codebronx
title: Work
permalink: /
---

<div class="site-shell">
  <section class="cb-intro">
    <p class="cb-kicker">CodeBronx / Work in learning + technology</p>
    <h1>Projects before pitches.</h1>
    <p class="cb-intro-copy">
      CodeBronx is a record of work across computing, STEM, AI, curriculum, physical computing,
      teacher learning, and student-centered design. The focus here is the work itself: what was
      built, what learners did, and what came from it.
    </p>
  </section>

  <section class="cb-section" id="work">
    <div class="cb-section-head">
      <h2>Selected Work</h2>
      <a class="cb-archive-link" href="{{ '/work/' | relative_url }}">View full archive</a>
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

  <section class="cb-collab" id="collaborate">
    <p class="cb-kicker">Collaborate</p>
    <h2>Building something that overlaps with this work?</h2>
    <p>
      CodeBronx occasionally collaborates with schools, universities, community organizations,
      and education teams on curriculum, learning design, emerging technology, and youth-centered STEM work.
    </p>
    <a class="cb-collab-link" href="{{ '/collaborate/' | relative_url }}">Start a conversation →</a>
  </section>

  <div class="cb-note">
    Project photography and artifacts will be added from original CodeBronx and partner work only.
  </div>
</div>
