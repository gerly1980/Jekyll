---
bg: "tag.jpg"
layout: page
title:  "infovis"
crawlertitle: "All tableau"
bg: "owl.jpg"
permalink: /infovis/
summary: "Posts about Web"
active: infovis
---

{% for post in site.posts limit: 15 %}
	{% if post.tags contains "infovis" %}
  <article class="index-page">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    {{ post.excerpt }}
  </article>
	{% endif %}
{% endfor %}