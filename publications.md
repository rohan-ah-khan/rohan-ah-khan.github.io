---
layout: page
title: Publications
nav: true
nav_order: 2
permalink: /publications/
---

<div class="posts">
  <div class="post">
    <h1 class="post-title">Publications</h1>

    {% assign pubs = site.posts | where_exp: 'p', 'p.categories contains "publication"' | sort: 'date' | reverse %}
    <ul class="pub-list">
      {% for post in pubs %}
        <li class="pub-item">
          {% if post.image %}
            <div class="pub-thumb">
              <img src="{{ post.image }}" alt="{{ post.title }}" loading="lazy">
            </div>
          {% endif %}
          <div class="pub-details">
            <h2 class="pub-title">
              {% if post.external_url %}
                <a href="{{ post.external_url }}" target="_blank" rel="noopener">{{ post.title }}</a>
              {% else %}
                <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
              {% endif %}
            </h2>
            <p class="pub-meta">
              {{ post.date | date: "%B %Y" }}
              {% if post.journal %} — <em>{{ post.journal }}</em>{% endif %}
            </p>
            <p class="pub-summary">
              {{ post.excerpt | strip_html | truncate: 220 }}
            </p>
          </div>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>

<style>
.pub-list { list-style: none; padding-left: 0; margin-top: 1.5rem; }
.pub-item {
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  margin-bottom: 2rem;
}
.pub-thumb img {
  width: 120px;
  height: auto;
  border-radius: 6px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}
.pub-details { flex: 1; }
.pub-title { font-size: 1.1rem; margin-bottom: 0.2rem; }
.pub-title a { text-decoration: none; }
.pub-meta { color: #666; font-size: 0.9rem; margin-bottom: 0.5rem; }
.pub-summary { color: #444; line-height: 1.5; }
@media (max-width: 600px) {
  .pub-item { flex-direction: column; align-items: center; text-align: center; }
  .pub-thumb img { width: 100%; max-width: 280px; }
}
</style>
