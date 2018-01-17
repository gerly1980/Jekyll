---
bg: "tag.jpg"
layout: page
permalink: /posts/infovis/
title: "可视化笔记"
crawlertitle: "All articles"
summary: "Posts about infovis"
active: note_infovis
---


{% for post in site.posts limit: 20 %}
	{% if post.tags contains "note_infovis" %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
	<span class="date">{{ post.date | date: "%d-%m-%Y"  }}</span>
	
	
		{{ post.excerpt }}
  </article>
	{% endif %}
{% endfor %}