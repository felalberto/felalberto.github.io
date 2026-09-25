---
layout: codebronx
title: Work
permalink: /
---

<div class="site-shell">
  <section class="cb-intro">
    <p class="cb-kicker">CodeBronx / Work in learning + technology</p>
    <h1>Learning Through Technology</h1>
    <p class="cb-intro-copy">
      CodeBronx documents how students and educators learn technology by using it: coding, building devices, experimenting with AI, prototyping ideas, and solving problems.
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
        {% capture card_class %}{% case forloop.index %}{% when 1 %}cb-featured{% when 2 %}cb-wide{% when 3 %}cb-narrow{% when 4 %}cb-editorial{% when 5 %}cb-narrow{% when 6 %}cb-wide{% when 7 %}cb-editorial{% endcase %}{% endcapture %}
        <a class="cb-project-card {{ card_class | strip }}" href="{{ post.url | relative_url }}">
          {% if post.image %}
            <img class="cb-project-image" src="{{ post.image | relative_url }}" alt="">
          {% endif %}

          <div class="cb-card-top cb-card-top-year-only">
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
        Across the projects, the idea is consistent: understand the technology, experiment with it, and figure out what you can make or solve with it.
      </p>
    </div>
  </section>

  <section class="cb-collab" id="collaborate">
    <p class="cb-kicker">Collaborate</p>
    <h2>Building something that overlaps with this work?</h2>
    <p>
      CodeBronx occasionally works with schools, universities, community organizations,
      and education teams on curriculum, STEM learning, AI, physical computing, and projects that give young people something real to build or investigate.
    </p>
    <a class="cb-collab-link" href="{{ '/collaborate/' | relative_url }}">Start a conversation →</a>
  </section>
</div>
