---
layout: default
title: Ideas
permalink: /ideas/
---
# Ideas

A collection of engineering essays on system design trade-offs, implementation strategy, and product-technical decision making.

<ul class="list-plain">
  {% assign idea_posts = site.posts | where_exp: "item", "item.categories contains 'ideas'" %}
  {% for post in idea_posts %}
  <li class="card">
    <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a><br />
    <small class="meta">{{ post.date | date: "%Y-%m-%d" }}</small>
  </li>
  {% endfor %}
  {% if idea_posts.size == 0 %}
  <li class="card">No essays have been published in this section yet.</li>
  {% endif %}
</ul>
