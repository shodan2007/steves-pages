{% assign recent_posts = site.posts | slice: 0, include.limit | default: 5 %}

<div class="recent-posts-grid">
  {% for post in recent_posts %}
    <div class="recent-post-card">
      {% if post.header.teaser %}
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}" class="recent-post-image">
        </a>
      {% endif %}
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="recent-post-date">{{ post.date | date: "%b %-d, %Y" }}</p>
      <p class="recent-post-excerpt">{{ post.excerpt }}</p>
    </div>
  {% endfor %}
</div>