---
bg: "tag.jpg"
layout: default
title:  "Web作品集"
permalink: /portfolio/
crawlertitle: "All Web"
summary: "Posts about Web"
active: portfolio
---


{% for post in site.posts limit: 10 %}
	{% if post.tags contains "portfolio" %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
	{% endif %}
{% endfor %}
