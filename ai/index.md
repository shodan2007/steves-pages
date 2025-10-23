---
layout: home
title: "AI"
permalink: /ai/
entries_layout: grid
classes: wide
category: ai

excerpt: "AI - Is that Artificial or Augmented Intelligence?"

sidebar:
  nav: "main"

header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: /assets/images/header.jpg
  caption: "Code clarity, prompt patterns, and lived experience"

read_time: true
share: true
---

{% assign ai_posts = site.posts | where_exp: "post", "post.categories contains 'AI'" %}
<div class="recent-posts-grid">
  {% for post in ai_posts %}
    <div class="recent-post-card">
      {% if post.header.teaser %}
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}" class="recent-post-image">
        </a>
      {% endif %}
      <div class="recent-post-text">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="recent-post-date">{{ post.date | date: "%b %-d, %Y" }}</p>
        <p class="recent-post-excerpt">{{ post.excerpt }}</p>
      </div>
    </div>
  {% endfor %}
</div>

## AI Prompt Patterns
Examples and notes from Coursera assignments and real prompts.

{% include feature_row id="quicknav" %}
