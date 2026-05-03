---
layout: default
title: Notes
permalink: /notes/
---

<section class="page-hero">
  <p class="eyebrow">DAILY LEARNING NOTES</p>
  <h1>Markdown-powered blog</h1>
  <p>Create one Markdown file per day in <code>_posts</code>. GitHub Pages will publish it automatically.</p>
</section>

<section class="post-list">
{% for post in site.posts %}
  <a class="note-row" href="{{ post.url }}">
    <small>{{ post.date | date: "%B %d, %Y" }}</small>
    <h3>{{ post.title }}</h3>
    {% if post.subtitle %}<p>{{ post.subtitle }}</p>{% endif %}
  </a>
{% endfor %}
</section>
