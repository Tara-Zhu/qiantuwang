# 相关代码已经修改调试
**实现：千图网上高清图片的爬取**

程序运行20小时，爬取大约162000张图片
## 笔记： ##

一、scrapy图片爬虫构建思路

     1.分析网站
     2.选择爬取方式与策略
     3.创建爬虫项目 → 定义items.py
     4.编写爬虫文件
     5.编写pipelines与setting
     6.调试

二、千图网难点（[http://www.58pic.com/](http://www.58pic.com/)）

     1.要爬取全站的图片
     2.要爬取高清的图片------找出高清地址即可
     3要有相应的反爬虫机制------如模拟浏览器，不记录cookie等，只要相应注释去掉即可COOKIES_ENABLED = False

三、散点知识

   	1.from scrapy.http import Request 是回调函数用Request(url=...,callback=...)
   	2.xpath的//表示提取所有符合的节点

----------
如果本项目对你有用请给我一颗star，万分感谢。

