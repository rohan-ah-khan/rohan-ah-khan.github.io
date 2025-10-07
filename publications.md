---
layout: default
title: Publications
nav: true
nav_order: 2
permalink: /publications/
---

<ul>
{%- assign pubs = site.posts | where_exp: 'p', 'p.categories contains "publication"' -%}
{%- for post in pubs -%}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {%- if post.venue or post.year -%}
      — {{ post.venue }}{%- if post.venue and post.year -%}, {% endif -%}{{ post.year }}
    {%- endif -%}
    {%- if post.authors -%}<br><small>{{ post.authors }}</small>{%- endif -%}
  </li>
{%- endfor -%}
</ul>
