---
layout: default
title: Home
---
# Engineering Notes and Commentary

Welcome to my personal blog. I publish focused technical commentary, lessons from production work, and long-form essays on software engineering decisions.

<div class="card">
  <h2>Editorial focus</h2>
  <ul>
    <li><strong>Technical News:</strong> analysis of notable releases, platform updates, and ecosystem shifts.</li>
    <li><strong>Ideas:</strong> architecture opinions, implementation proposals, and technical essays.</li>
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
