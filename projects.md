---
layout: page
title: Projects
permalink: /projects/
---

<ul class="project-list">
  {% for project in site.projects %}
    <li class="project-list-item">
      <p>
        <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
      </p>
      {{ project.excerpt }}
    </li>
  {% endfor %}
</ul>
