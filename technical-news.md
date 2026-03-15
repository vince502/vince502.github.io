---
layout: default
title: News
permalink: /technical-news/
---
# News

Concise analysis of relevant releases, standards updates, and product announcements across the software ecosystem.

<ul class="list-plain">
  {% assign news_posts = site.posts | where_exp: "item", "item.categories contains 'technical-news'" %}
  {% for post in news_posts %}
  <li class="card">
    <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a><br />
    <small class="meta">{{ post.date | date: "%Y-%m-%d" }}</small>
  </li>
  {% endfor %}
  {% if news_posts.size == 0 %}
  <li class="card">No technical news brief has been published yet.</li>
  {% endif %}
</ul>
