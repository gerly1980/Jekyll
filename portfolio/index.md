---
layout: default
bg: "tag.jpg"
title: "信息可视化作品集"
permalink: /what/
summary: "Posts about infovis"
active: what
---


<html class="no-js" lang="zh-CN">
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width">
<link rel="stylesheet" href="/portfolio/style.css">
</head>
<body>
<img src="/portfolio/image/exam.png" alt="The picture of blog page" width="100%" height="90px">
<div class="flexbox-container">
	<div class="left" >
		
* 交通设施分布情况：<br>飞机场和火车站分布最广，高铁和地铁设施集中在东部地区。汽车站数量最多。
<img src="/portfolio/image/fenbu.png" alt="The picture of blog page" width="350px" height="400px">
<br>- 三大地带比较：<br>东部地带各类设施拥有率最高
	</div>
	<div class="right">
* 各城市比较：<br>北上广的交通设施拥有数量最高，西藏等偏远城市数量较少
<img src="/portfolio/image/shuliang.jpg" alt="The picture of blog page" width="300px" height="250px">

* 交通设施缺少情况：<br>北上广的交通设施拥有数量最高，西藏等偏远城市数量较少
<img src="/portfolio/image/none.jpg" alt="The picture of blog page" width="300px" height="150px">

	</div>
</div>
{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% if tag contains 'infovis' %}
  <h3 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h3>
{% endif %}
  <ul class="year">
    {% for post in posts %}
      {% if post.tags contains "infovis" %}
        <li>
          {% if post.lastmod %}
            <a href="{{ post.url | relative_url}}">{{ post.title }}</a>
            <span class="date">{{ post.lastmod | date: "%d-%m-%Y"  }}</span>
          {% else %}
            <a class="infovis" href="{{ post.url | relative_url}}">{{ post.title }}:{{ post.description }}</a>
          {% endif %}
        </li>
      {% endif %}
    {% endfor %}
  </ul>
{% endfor %}
</body>
</html>