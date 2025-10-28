---
layout: single
title: "Code That Cares: Building Ethical AI for Mental Health"
entries_layout: grid

header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: /assets/images/header.jpg
  caption: "People first. Systems that support, not just scale."
  excerpt: "People first. Systems that support, not just scale (2)"

---

In a world where software shapes lives, I build systems that listen. This portfolio blends technical precision with human-centered design — from trauma-aware flows to ethical AI demos. Whether you're debugging resilience or architecting trust, you'll find tools here that prioritize clarity, care, and real-world impact.

<div class="recent-posts-grid">
  {% for post in site.posts %}
    <div class="recent-post-card" 
       style="border: 1px solid #e0e0e0; 
            background-color: #fffaf0;
            border-radius: 12px; 
            padding: 16px; 
            margin: 12px 0; 
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
            transition: transform 0.2s ease, box-shadow 0.2s ease;"
        onmouseover="this.style.transform='translateY(-4px)';this.style.boxShadow='0 6px 12px rgba(0,0,0,0.15)';"
        onmouseout="this.style.transform='none';this.style.boxShadow='0 2px 6px rgba(0,0,0,0.1)';">
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

    <hr>

  {% endfor %}
</div>