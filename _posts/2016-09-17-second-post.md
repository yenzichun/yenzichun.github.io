---
layout: post
title:  Second Post
date: "2016-09-17 03:42:44"
published: true
tags: [example1, example2]
---

Your markdown here!


{% highlight r %}
plot(1:10)

options(digits = 3)
cat("hello world!")

set.seed(123)
(x=rnorm(40)+10)

knitr::kable(head(mtcars))

par(mar = c(4,4,0.1,0.1))
plot(cars,pch=19,col="red")

$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$
{% endhighlight %}



{% highlight text %}
## Error: <text>:14:1: 未預期的 '$'
## 13: 
## 14: $
##     ^
{% endhighlight %}
