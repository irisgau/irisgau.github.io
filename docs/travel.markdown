---
layout: page
title: Travel
permalink: /travel/
---

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "travel" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>