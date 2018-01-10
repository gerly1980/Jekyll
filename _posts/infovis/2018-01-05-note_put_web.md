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
	



* 在 iFrame 中嵌入 Tableau Public 视图时，URL 必须包括以下参数：

```
showVizHome=no 
embed=true 
```
下面的示例演示可用于在 iFrame 中嵌入 Tableau Public 视图的代码，其中来源 (src) 为视图的 URL：
```
<iframe src="http://public.tableausoftware.com/views/public_exercise/Dashboard1?:showVizHome=no&:embed=true"
 width="645" height="955"></iframe>
```
 注意：将视图的 URL 用于 iframe src 属性时，不要包括 URL 最末尾的数字符号 (#) 和数字。
```
正确的 src 内容：
https://public.tableausoftware.com/views/public_exercise/Dashboard1?:showVizHome=no&:embed=true
不正确的 src 内容：
https://public.tableausoftware.com/views/public_exercise/Dashboard1?:showVizHome=no&:embed=true#2
```
* 为确保默认情况下在嵌入视图中显示原始视图，请确保名称参数的嵌入代码 URL 未显式引用自定义视图，并在嵌入代码中包含以下筛选器参数：<param name="filter" value=":original_view=yes"/>



<a href="http://kb.tableau.com/articles/howto/embedding-tableau-public-views-in-iframes?lang=zh-cn">详情可见：在 iFrame 中嵌入 Tableau Public 视图</a>
