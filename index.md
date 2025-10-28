---
layout: single
title: "Code That Cares"
entries_layout: grid

header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: /assets/images/homeheader.jpg
  caption: "Ethical AI, Software, and Listening - for <i>Our</i> Mental Health"

excerpt: "People first. Systems that support, not just scale."

---

I don’t just build systems that listen — I listen. I’ve led behavioral health technicians supporting unhoused individuals, managed addiction recovery homes, and worked in psychiatric inpatient care. With an MS in Industrial Engineering, decades as a professional software developer, peer support certification, lived experience, and graduate-level psychology coursework, I bring both technical depth and human insight. As a developer, architect, and engineer, I design trauma-aware tools, ethical AI flows, and resilient systems that serve real people. Whether you’re debugging code or navigating anger, I’m here to help with clarity, care, and calm.

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