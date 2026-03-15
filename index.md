---
layout: default
title: Home
---
# Welcome

teo my personal blog. Here I post, discuss whatever interest me

<div class="card">
  <h2>Editorial focus</h2>
  <ul>
    <li><strong>News:</strong> New stories that I find interesting</li>
    <li><strong>Ideas:</strong> Experiment, Technological challenge.</li>
    <li><strong>Experience:</strong> practical retrospectives on delivery, reliability, and team execution.</li>
    <li><strong>CV:</strong> a concise overview of my background, capabilities, and project impact.</li>
  </ul>
</div>

## Latest posts

<ul class="list-plain">
  {% assign posts = site.posts | slice: 0, 8 %}
  {% for post in posts %}
  <li class="card">
    <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a><br />
    <small class="meta">{{ post.date | date: "%Y-%m-%d" }}{% if post.categories.size > 0 %} · {{ post.categories | join: ", " }}{% endif %}</small>
  </li>
  {% endfor %}
  {% if site.posts.size == 0 %}
  <li class="card">No articles published yet. Create your first post in <code>_posts/</code>.</li>
  {% endif %}
</ul>
