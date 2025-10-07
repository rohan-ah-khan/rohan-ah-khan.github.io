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
        </li>
      {% endfor %}
    </ul>
  </div>
</div>

<style>
.pub-list { list-style: none; padding-left: 0; margin-top: 1.5rem; }
.pub-item { margin-bottom: 2rem; }
.pub-title { font-size: 1.1rem; margin-bottom: 0.2rem; }
.pub-title a { text-decoration: none; }
.pub-meta { color: #666; font-size: 0.9rem; margin-bottom: 0.5rem; }
.pub-summary { color: #444; line-height: 1.5; }
</style>
