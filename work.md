---
layout: codebronx
title: Work Archive
permalink: /work/
---

<div class="site-shell">
  <section class="archive-intro">
    <p class="cb-kicker">Archive</p>
    <h1>The work, in one place.</h1>
    <p>
      Projects, curriculum, professional learning, AI, physical computing, and student-centered technology work.
    </p>
  </section>

  <section class="archive-list">
    {% assign portfolio = site.categories.Portfolio %}
    {% for post in portfolio %}
      <a class="archive-item" href="{{ post.url | relative_url }}">
        <div class="archive-year">{{ post.date | date: "%Y" }}</div>

        <div>
          <h2 class="archive-title">{{ post.title }}</h2>
          <p class="archive-excerpt">
            {% if post.description %}
              {{ post.description }}
            {% elsif post.excerpt %}
              {{ post.excerpt | strip_html | strip_newlines | truncate: 220 }}
            {% endif %}
          </p>
        </div>

        <div class="archive-meta">
          {% if post.tags %}
            {% for tag in post.tags limit: 3 %}
              {{ tag }}{% unless forloop.last %}<br>{% endunless %}
            {% endfor %}
          {% endif %}
        </div>
      </a>
    {% endfor %}
  </section>
</div>
