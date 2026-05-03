---
layout: default
title: Home
---

<section class="hero">
  <div class="hero-content">
    <p class="eyebrow">DATA SCIENCE • AI • DECISION INTELLIGENCE</p>
    <h1>Turn Data Into Decisions</h1>
    <p>
      Practical notes, visual explainers, and frameworks for data science, analytics, machine learning, and credit risk.
    </p>

    <div class="hero-actions">
      <a href="#latest" class="btn-primary">Explore Notes</a>
      <a href="#topics" class="btn-secondary">Browse Topics</a>
    </div>
  </div>
</section>

<section id="topics" class="topics">
  <h2>Learning Topics</h2>

  <div class="topic-grid">
    <a class="topic-card" href="/categories/data-science">
      <span>01</span>
      <h3>Data Science</h3>
      <p>Python, statistics, modeling, experiments, and analytics workflow.</p>
    </a>

    <a class="topic-card" href="/categories/ai">
      <span>02</span>
      <h3>AI & Machine Learning</h3>
      <p>ML systems, generative AI, LLMs, model evaluation, and deployment.</p>
    </a>

    <a class="topic-card" href="/categories/analytics">
      <span>03</span>
      <h3>Business Analytics</h3>
      <p>Decision-making, dashboards, segmentation, and growth analytics.</p>
    </a>

    <a class="topic-card" href="/categories/credit-risk">
      <span>04</span>
      <h3>Credit Risk</h3>
      <p>PD, LGD, scorecards, early warning, approval strategy, and model governance.</p>
    </a>
  </div>
</section>

<section id="latest" class="latest">
  <h2>Latest Notes</h2>

  <div class="post-grid">
    {% for post in site.posts %}
      <a class="post-card" href="{{ post.url }}">
        <p class="post-meta">{{ post.date | date: "%b %d, %Y" }}</p>
        <h3>{{ post.title }}</h3>

        {% if post.subtitle %}
        <p>{{ post.subtitle }}</p>
        {% endif %}

        <div class="tag-row">
          {% for category in post.categories %}
            <span>{{ category }}</span>
          {% endfor %}
        </div>
      </a>
    {% endfor %}
  </div>
</section>
