---
bg: "tag.jpg"
layout: default
title:  "portfolio"
permalink: /portfolio/
crawlertitle: "All Web"
summary: "Posts about Web"
active: portfolio
---
# This is my Web portfolio!

{% for post in site.posts limit: 10 %}
	{% if post.tags contains "portfolio" %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
	{% endif %}
{% endfor %}
