---
layout: post
title: "Github pages + Jekyll Bootstrap 靜態blog建置筆記"
description: "my first blog post"
category: Notes
tags: [Github, Jekyll]
---
{% include JB/setup %}


###前言###

以前就知道可以把github當blog用，不過一直不知道要從哪下手，也沒有需求跟動力．．．直到最近想要把在coursera上課的筆記跟一些code整理起來，才開始研究，而在過程中發現「其實還頗複雜的啊」！

以下是學習筆記：

1. 安裝`Ruby`、`RubyDevKit`、`Jekyll`、`Jekyll Bootstrap` trouble shooting:
	- RubyDevKit安裝失敗: 在RubyDevKit資料夾裡的`_config.yml` 檔案中新增路徑指向ruby的連結`C:/Ruby"`

2. 在github上建立repo

3. 安裝rdiscount (解析markdown用,但感覺沒必要)
4. 安裝 rouge ([網路](http://jekyll-windows.juthilo.com/3-syntax-highlighting/)上查到說可取代Pygments作為syntax highlighter)
5. 在`_config.yml` 把rouge設為 syntax highlighter `highlighter: rouge`

6. 安裝完Jekyll Bootstrap 後，第一個需要修改的設定檔是`_config.yml`，包括 title 及 author 等網站基本資料。

>	rake page           # Create a new page.
	rake post           # Begin a new post in ./_posts
	rake preview        # Launch preview environment

輸入「rake preview」即可建立預覽專用的伺服器，預設的 Port 號碼為 4000，所以用瀏覽器打開「http://localhost:4000/」即可預覽。之後新增、修改網頁內容，都可以重新整理瀏覽器網頁，查看更新的結果（需要等待 Jekyll 在背景產生好靜態網站）。

資料夾下的 index.md、tags.html、archive.html、categories.html、pages.html 是一些預設的基本頁面，可以直接修改內容，這些檔案的內容採用 Markdown 格式編寫。檔首的 --- 區塊有 title 等設定，是 Jekyll 網頁的特殊設定方式。

* [Markdown](http://markdown.tw/)

7. 建立新網頁：

rake page title="about me"

或

rake post title="hello world"

使用 page 或 post，必須看新增的網頁內容是屬於頁面（page）或文章（post）類型，舉例來說，「關於本站」、「作者介紹」這種不會經常發佈、固定式的資料，就是用 page，而「新聞」、「活動」等日後會常發佈新內容的類型，就是 post。

建立或修改網頁內容後，使用 git 將目前的版本提交。

>	git add .
	git commit . -m 'just another commit'
	git push origin master

之後專案就會更新，使用「http://github.com/USERNAME/USERNAME.github.com」可以看一下專案更新結果。通常只需要等待片刻時間（第一次發佈會比較久），就可以從「http://USERNAME.github.com」瀏覽已發佈的網站。 
	



- jekyll documentation
	[http://jekyllrb.com/docs/configuration/](http://jekyllrb.com/docs/configuration/)
- jekyllbootstrap
	[http://jekyllbootstrap.com/usage/jekyll-quick-start.html](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)
- install jekyll on windows
	[http://jekyll-windows.juthilo.com/1-ruby-and-devkit/](http://jekyll-windows.juthilo.com/1-ruby-and-devkit/)
- jekyll & jekyll bootstrap 簡潔介紹(包含work flow 好懂)
	[http://blog.lyhdev.com/2012/02/jekyll-github-pages.html](http://blog.lyhdev.com/2012/02/jekyll-github-pages.html)
- 詳盡的解釋Jekyll各配置參數
	[http://beiyuu.com/github-pages/](http://beiyuu.com/github-pages/)
- 三分鐘建立一個Jekyll Blog(使用lanyon模板)
	[http://ztpala.com/2012/01/12/zero-to-hosted-jekyll-blog-in-3-minutes/](http://ztpala.com/2012/01/12/zero-to-hosted-jekyll-blog-in-3-minutes/)
- windows下本地jekyll博客搭建手记(主要是ruby&jekyll搭建筆記,還有一些trouble shooting) 
	[http://blog.jsfor.com/skill/2013/09/07/jekyll-local-structures-notes/
](http://blog.jsfor.com/skill/2013/09/07/jekyll-local-structures-notes/
)
- 教學文(主要是有一些不錯的模板)
	[http://dlyang.me/blog-migrate/](http://dlyang.me/blog-migrate/)