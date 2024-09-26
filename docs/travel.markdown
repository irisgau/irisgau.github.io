---
layout: page
title: Travel
permalink: /travel/
---

I have quite a poor memory when it comes to travel, which feels especially unfortunate since exploring new places is something I truly love. I've been fortunate enough to visit many places in my lifetime. To capture those experiences, I’ve started writing travel blogs. Not only does it help me preserve those memories, but if it can inspire or help others in planning their own adventures, all the better.

<ul class="post-list">
  {% for post in site.posts %}
    {% if post.categories contains "travel" %}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
        {%- endif -%}
      </li>
    {% endif %}
  {% endfor %}
</ul>