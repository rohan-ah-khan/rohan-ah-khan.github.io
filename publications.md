---
layout: page
title: Publications
nav: true
nav_order: 2
permalink: /publications/
---

<div class="posts">
  <div class="post">
    <p>Below is a selection of research publications and scholarly works.</p>
    <hr>

    <ul class="pub-list">
      {% assign pubs = site.posts | where_exp: 'p', 'p.categories contains "publication"' %}
      {% for post in pubs %}
        <li>
          <strong><a href="{{ post.url | relative_url }}">{{ post.title }}</a></strong><br>
          {% if post.venue or post.year %}
            <em>{{ post.venue }}</em>{% if post.venue and post.year %}, {% endif %}{{ post.year }}.<br>
          {% endif %}
          {% if post.authors %}
            <small>{{ post.authors }}</small><br>
          {% endif %}
          {% if post.summary %}
            <small>{{ post.summary }}</small><br>
          {% endif %}
          {% if post.links %}
            <small>
              {% if post.links.pdf %}<a href="{{ post.links.pdf }}">PDF</a>{% endif %}
              {% if post.links.doi %}{% if post.links.pdf %} · {% endif %}<a href="{{ post.links.doi }}">DOI</a>{% endif %}
            </small>
          {% endif %}
        </li>
      {% endfor %}
    </ul>
  </div>
</div>

<style>
.pub-list { list-style: none; padding-left: 0; margin-top: 1.5rem; }
.pub-list li { margin-bottom: 1.5rem; line-height: 1.6; }
.pub-list strong { font-size: 1.05rem; }
.pub-list em { color: #666; }
.pub-list small { color: #555; display: block; }
</style>
