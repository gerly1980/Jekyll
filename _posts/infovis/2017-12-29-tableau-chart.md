---
layout: post
bg: "infovis.jpg"
title:  "如何将tableau作品嵌入网页"
crawlertitle: "notebook about tableau"
summary: "把作品分享到Web？"
date: 2017-12-29
tags: "note_infovis"
categories:
  - posts
  - infovis

---
笔记记载如何将tableau作品嵌入网页.
具体步骤：
	* 在tableau public 申请个人账号
	* 把tableau的作品存到tableau public（点击Tableau server）
	* 此时网页会弹窗出来你的tableau public的网址。（在工作表或仪表盘的右下角有个分享的按钮）
	
<iframe>的嵌入方法
<iframe src="https://public.tableau.com/shared/BRJX6KCMZ?:display_count=yes/Dashboard1?:showVizHome=no&:embed=true" width="760px" height="900px" frameborder="0"></iframe>
``` Dashboard1?:showVizHome=no&:embed=true``` 这段是固定的，把的网址往前面贴。



* 使用共享嵌入代码：每个视图顶部的共享链接可以复制和粘贴到网页中的嵌入代码。
* 编写自己的嵌入代码：增强tableau提供的嵌入代码，或者生成自己的代码。
* 使用tableau javascript API：可以在自己的web应用程序代码中使用 



