---
bg: "tag.jpg"
layout: page
permalink: /posts/rwd/
title: "posts"
crawlertitle: "All articles"
summary: "Posts about rwd"

---

{% for post in site.posts limit: 5 %}
	{% if post.tags contains "note_rwd" %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
	{% endif %}
{% endfor %}