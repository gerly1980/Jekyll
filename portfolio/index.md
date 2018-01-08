---
layout: default
bg: "tag.jpg"
title: "学生作品集"
permalink: /what/
modified:
excerpt: "展示学生作品集，好的丶可改进的及有趣的"
tags: []
image: 
  feature: 
  teaser: Portfolio.svg
active: what
---


<html class="no-js" lang="zh-CN">
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width">
<link rel="stylesheet" href="/portfolio/style.css">
</head>
<body>
<div class="flexbox-container">
	<div class="left" >
<div class="col-sm-7" markdown="1"><!-- left -->
##### 交通设施分布情况：
飞机场和火车站分布最广，高铁和地铁设施集中在东部地区。汽车站数量最多。
##### 三大地带比较：
东部地带各类设施拥有率最高
<img src="/portfolio/image/fenbu.jpg" alt="The picture of blog page" width="360px" height="400px">

</div> 
	</div>
	<div class="right">
* 各城市比较：
北上广的交通设施拥有数量最高，西藏等偏远城市数量较少
<img src="/portfolio/image/shuliang.jpg" alt="The picture of blog page" width="300px" height="300px">

- 交通设施缺少情况：
就珠江三角洲地区来看，数量最多的体育休闲服务分布最广。
公司企业集中在深圳；生活服务多在广州，东莞两类各一点。
政府机构及社会团体方面，就一点在广州。
<img src="/portfolio/image/none.jpg" alt="The picture of blog page" width="300px" height="200px">

	</div>
</div>
{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% if tag contains 'note_rwd' %}
  <h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2>
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
</body>
</html>