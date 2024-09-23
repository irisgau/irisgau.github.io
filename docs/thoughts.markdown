---
layout: page
title: Thoughts
permalink: /thoughts/
---

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "thoughts" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>