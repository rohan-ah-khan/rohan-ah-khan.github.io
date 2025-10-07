---
layout: page
title: Publications
nav: true
nav_order: 2
permalink: /publications/
---

<div class="posts">
  <div class="post">
    <p>Below is a selection of research publications and scholarly work I have contributed to recently.</p>
    <hr>

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

          <div class="pub-body">
            {% if post.summary %}
              {{ post.summary }}
            {% else %}
              {{ post.content }}
            {% endif %}
          </div>

          {% if post.image %}
            <div class="pub-thumb">
              {% if post.external_url %}
                <a href="{{ post.external_url }}" target="_blank" rel="noopener">
                  <img src="{{ post.image }}" alt="{{ post.title }}" loading="lazy">
                </a>
              {% else %}
                <img src="{{ post.image }}" alt="{{ post.title }}" loading="lazy">
              {% endif %}
            </div>
          {% endif %}
        </li>
      {% endfor %}
    </ul>
  </div>
</div>

<style>
.pub-list { list-style: none; padding-left: 0; margin-top: 1.25rem; }
.pub-item { margin-bottom: 2.25rem; }
.pub-title { font-size: 1.1rem; margin-bottom: 0.2rem; }
.pub-title a { text-decoration: none; }
.pub-meta { color: #666; font-size: 0.9rem; margin-bottom: 0.6rem; }
.pub-body { color: #444; line-height: 1.6; }
.pub-thumb { margin-top: 0.75rem; }
.pub-thumb img { max-width: 100%; height: auto; display: block; border-radius: 6px; box-shadow: 0 2px 6px rgba(0,0,0,0.08); }
</style>
