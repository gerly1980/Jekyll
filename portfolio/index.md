---
layout: default
bg: "tag.jpg"
title: "信息可视化作品集"
permalink: /what/
summary: "Posts about infovis"
active: what
---



<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width">
<link rel="stylesheet" href="/portfolio/style.css">
</head>
<body>
<a href="/infovis/infovis-final-exam/"><img src="/portfolio/image/exam.png" alt="The picture of blog page" width="100%" height="90px"></a>
<div class="flexbox-container">
	<div class="left" >
		
三大地带交通设施分布情况：<br>* 飞机场和火车站分布在各地区，高铁和地铁设施集中在东部地区。
<a href="/infovis/infovis-final-exam/"><img src="/portfolio/image/fenbu.png" alt="The picture of blog page" width="350px" height="250px"></a>

各城市比较：<br>* 广东省和黑龙江省的拥有量排行在Top5内<br>* 地铁站和高铁站覆盖率并不可观
<a href="/infovis/infovis-final-exam/"><img src="/portfolio/image/shuliang.png" alt="The picture of blog page" width="350px" height="200px"></a>
	</div>
	<div class="right">

交通运输产值情况：<br>* 广东省交通产值具首位，其次是江苏省和山东省<br>* 交通运输产值逐年递增,交通产业发展可观。
<a href="/infovis/infovis-final-exam/"><img src="/portfolio/image/sandian.png" alt="The picture of blog page" width="300px" height="400px"></a>
交通设施数量与交通运输产值的关系：<br>* P值<.0001,达到显著，成相关关系<br>* 交通越发达地区，交通产值越高
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
          {% else %}
            <a class="infovis" href="{{ post.url | relative_url}}">{{ post.title }}>{{ post.description }}</a>
          {% endif %}
        </li>
      {% endif %}
    {% endfor %}
  </ul>
{% endfor %}
</body>