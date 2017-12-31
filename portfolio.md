---
bg: "tag.jpg"
layout: default
title:  "Web"
permalink: /portfolio/
crawlertitle: "All Web"
summary: "Posts about Web"
active: portfolio
---
helloaaaaa

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% if tag contains 'jekyll' %}
  <h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2>
{% endif %}

  <ul class="year">
    {% for post in posts %}
      {% if post.tags contains 'jekyll' %}
        <li>
          {% if post.lastmod %}
		  <h1>{{post.title}}</h1>
            <a href="{{ post.url | relative_url}}">{{ post.title }}</a>
            <span class="date">{{ post.lastmod | date: "%d-%m-%Y"  }}</span>
          {% else %}
            <a href="{{ post.url | relative_url}}">{{ post.title }}</a>
            <span class="date">{{ post.date | date: "%d-%m-%Y"  }}</span>
          {% endif %}
        </li>
      {% endif %}
    {% endfor %}
  </ul>

{% endfor %}
