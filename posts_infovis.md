---
bg: "tag.jpg"
layout: page
permalink: /posts/infovis/
title: "posts"
crawlertitle: "All articles"
summary: "Posts about infovis"

---

{% for post in site.posts limit: 10 %}
	{% if post.tags contains "note_infovis" %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
	{% endif %}
{% endfor %}