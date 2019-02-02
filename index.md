---
layout: default
title: Home
---
<h1>Latest Posts</h1>
<ul class="latest-post-list">
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a><span class="post-date"> - {{ post.date | date_to_string}}</span></h2>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>