---
layout: default
title: Home
---

<section class="hero">
  <p class="eyebrow">DATA SCIENCE • AI • ANALYTICS</p>

  <h1>Turn Data Into Decisions</h1>

  <p class="hero-text">
    Practical notes on data science, machine learning, analytics, and decision intelligence.
  </p>
</section>

<section class="posts-section">
  <h2>Latest Notes</h2>

  <div class="post-grid">
    {% for post in site.posts %}
      <a class="post-card" href="{{ post.url }}">
        <p class="post-date">{{ post.date | date: "%b %d, %Y" }}</p>
        <h3>{{ post.title }}</h3>

        {% if post.subtitle %}
        <p>{{ post.subtitle }}</p>
        {% endif %}
      </a>
    {% endfor %}
  </div>
</section>
