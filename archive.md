---
bg: "tag.jpg"
layout: page
permalink: /posts/
title: "文章"
crawlertitle: "All articles"
summary: "Posts about all"
active: archive
---

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% if tag contains 'note_rwd' %}
  <div><a href="/posts/rwd/"><h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2></a></div>
{% endif %}
  <ul class="year">
    {% for post in posts %}
      {% if post.tags contains "note_rwd" %}
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

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% if tag contains 'note_infovis' %}
  <div><a href="/posts/infovis/"><h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2></a></div>
{% endif %}
  <ul class="year">
    {% for post in posts %}
      {% if post.tags contains "note_infovis" %}
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

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% if tag contains 'note_wsg' %}
  <h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2>
{% endif %}
  <ul class="year">
    {% for post in posts %}
      {% if post.tags contains "note_wsg" %}
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