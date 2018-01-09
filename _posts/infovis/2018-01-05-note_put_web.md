---
layout: post
title: "将tableau作品嵌入网页"
date: 2017-12-30
description: ”如何将tableau作品嵌入网页“
author: "zhihao"
tags: "note_infovis"
categories:
  - posts
  - infovis
 
---




* 具体步骤：	

	* 在tableau public 申请个人账号
	* 在desktop界面选择发布。菜单“服务器”--“发布工作簿”
	* 此时网页会弹窗出来你的tableau public的网址。（在工作表或仪表盘的右下角有个分享的按钮）
	* 直接访问tableau server中已经发布好的图表
	* 在仪表盘右下方会有个分享按钮，选择你需要的插入方式。
	
* script插入方式，直接复制粘贴在你需要放置的HTML档里就可以了。
	
* ··· <iframe>···嵌入方式
```
	<iframe src="https://public.tableau.com/shared/BRJX6KCMZ?:display_count=yes/Dashboard1?:showVizHome=no&:embed=true" width="760px" height="900px" frameborder="0">
 Dashboard1?:showVizHome=no&:embed=true /*这段是固定的，把你的网址往前面贴。*/
```



<a href="https://jingyan.baidu.com/article/39810a238976e7b636fda6c4.html">可点击此处见详情</a>