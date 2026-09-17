---
layout: page
title: Blog
published: false
---
<p class="section-intro">Outreach-style notes on research trends and my own work.</p>

<ul class="post-list">
{% for post in site.posts %}
  <li class="post-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date: "%B %-d, %Y" }}</span>
  </li>
{% endfor %}
</ul>
