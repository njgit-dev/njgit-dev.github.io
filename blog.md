---
layout: page
title: Blog
permalink: /blog/
---

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-list-item">
      <p>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
        <small class="post-list-date">{{ post.date | date: "%B %-d, %Y" }}</small>
      </p>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
