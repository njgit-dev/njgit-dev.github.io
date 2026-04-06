---
layout: page
title: Home
---

<section class="home-intro">
  <p>Welcome to the site.</p>
  <p>This is a simple Jekyll publishing site for writing, projects, and ideas.</p>
</section>

<section class="home-posts">
  <h2>Latest Posts</h2>

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
</section>
