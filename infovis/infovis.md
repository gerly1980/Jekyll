---
bg: "tag.jpg"
layout: default
title:  "infovis"
crawlertitle: "All tableau"
bg: "owl.jpg"
permalink: /infovis/
summary: "Posts about Web"
active: infovis
---
# This is my Tableau portfolio!

{% for post in site.posts limit: 5 %}
	{% if post.tags contains "infovis" %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
	{% endif %}
{% endfor %}