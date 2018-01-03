---
layout: post
bg: "tools.jpg"
title:  "blog page power by RWD example"
crawlertitle: "blog page"
summary: "blog page power by RWD example"
date: 2017-12-30	
tags: "portfolio"
categories:
  - portfolio
---

<img src="/portfolio/image/page.jpg" alt="The picture of blog page"/>


<html lang="en">
<link rel="stylesheet" href="/portfolio/styles.css">
<head>
	<link href='http://fonts.googleapis.com/css?family=Oswald:700' rel='stylesheet' type='text/css'>
	<meta charset="utf-8">
	<title>Layout example</title>
	<meta name="viewport" content="width=device-width">
	

</head>

<body>
	<div class="MenuWrap">
		<a href="#" id="logobox" class="LastItem">My blog</a>
		<a href="#" class="ListItem">Home</a>
		<a href="#" class="ListItem">Tableau</a>
		<a href="#" class="ListItem">RWD</a>
		<a href="#" class="ListItem">About us</a>
	</div>
<!--banner-->
	<div class="banner">
	<!--menu-->

		<div class="pstyle">
			<p>Hello, I'm python hao<br>This is my blog !<a href="#C4" id="beginbox">click</a></p>

		</div>
	</div>
<!--section-->
	<div class="FlexWrapper">
		<!--header-->
		<div class="FlexItems FlexHeader">
			<div class="spstyle"><p><a name="C4"></a>  follow</p></div>
		</div>
		<!--section tableau-->
		<div class="FlexItems FlexContentOne">
			<!--tableau content-->
			<nav class="Scroll_Wrapper">
		<figure class="Item">
			<img src="/portfolio/image/f1.jpg" alt="Guardians of the Galaxy"/>
			<figcaption class="Caption">Guardians of the Galaxy</figcaption>
		</figure>
		<figure class="Item">
			<img src="/portfolio/image/f2.jpg" alt="The Hunger Games: Mockingjay - Part 1"/>
			<figcaption class="Caption">The Hunger Games: Mockingjay - Part 1</figcaption>
		</figure>
		<figure class="Item">
			<img src="/portfolio/image/f3.jpg" alt="Captain America: The Winter Soldier"/>
			<figcaption class="Caption">Captain America: The Winter Soldier</figcaption>
		</figure>
			</nav>
		</div>
		<div class="FlexItems FlexSideOne">
			<div class="spstyle"><p>This my tableau homework.</p></div>
		</div>
			
		<!--section notebook-->
		<div class="FlexItems FlexSideTwo">
			<div class="spstyle"><p>I am notebook</p></div>
		</div>
		<!--notebook content-->	
		<div class="FlexItems FlexContentTwo">
					<nav class="Scroll_Wrapper">
		<figure class="Item">
			<img src="/portfolio/image/f4.jpg" alt="Guardians of the Galaxy"/>
			<figcaption class="Caption">Guardians of the Galaxy</figcaption>
		</figure>
		<figure class="Item">
			<img src="/portfolio/image/f2.jpg" alt="The Hunger Games: Mockingjay - Part 1"/>
			<figcaption class="Caption">The Hunger Games: Mockingjay - Part 1</figcaption>
		</figure>
		<figure class="Item">
			<img src="/portfolio/image/f3.jpg" alt="Captain America: The Winter Soldier"/>
			<figcaption class="Caption">Captain America: The Winter Soldier</figcaption>
		</figure>
			</nav>
		</div>

	</div>
		<!--footer-->
	<div class="FlexItems FlexFooter">
	<p class="footpstyle">© 2017  powered by <a href="http://www.ituring.com.cn/book/1817"> RWD</a></p>
	</div>
  


</body>
</html>