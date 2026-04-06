---
layout: page
title: Blog
permalink: /blog/
---

<ul>
  {% for post in site.posts %}
    <li>
      <p>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
        <small>{{ post.date | date: "%B %-d, %Y" }}</small>
      </p>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
