---
layout: page
title: Blog
permalink: /blog/
---

{%- if site.posts.size == 0 -%}
  <h2>No posts yet, check back soon!</h2>
{%- endif -%}

<ul>
{%- if site.posts.size > 0 -%}
  {% for post in site.posts %}
    <li>  
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
{%- endif -%}
</ul>
