---
layout: page
title: Blog
permalink: /blog/
---

<div class="page-card">
  <h2>Recent writing</h2>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="post-date">{{ post.date | date: "%B %-d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</div>
