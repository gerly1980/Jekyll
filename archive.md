---
bg: "tag.jpg"
layout: page
permalink: /posts/
title: "posts"
crawlertitle: "All articles"
summary: "Posts about all"
active: archive
---
# I am notebook of RWD!
{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% if tag contains 'rwd' %}
  <h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2>
{% endif %}
  <ul class="year">
    {% for post in posts %}
      {% if post.tags contains "rwd" %}
        <li>
          {% if post.lastmod %}
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
<br>
# I am notebook of tableau!
{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% if tag contains 'infovis' %}
  <h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2>
{% endif %}
  <ul class="year">
    {% for post in posts %}
      {% if post.tags contains "infovis" %}
        <li>
          {% if post.lastmod %}
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