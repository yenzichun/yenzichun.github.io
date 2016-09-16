---
layout: post
title:  Second Post
date: "2016-09-17 03:34:15"
published: true
tags: [example1, example2]
---

Your markdown here!


{% highlight r %}
plot(1:10)
{% endhighlight %}

![plot of chunk unnamed-chunk-1](https://dl.dropboxusercontent.com/u/59373967/jekyll/2016-09-17-second-post/unnamed-chunk-1-1.png)

{% highlight r %}
options(digits = 3)
cat("hello world!")
{% endhighlight %}



{% highlight text %}
## hello world!
{% endhighlight %}



{% highlight r %}
set.seed(123)
(x=rnorm(40)+10)
{% endhighlight %}



{% highlight text %}
##  [1]  9.44  9.77 11.56 10.07 10.13 11.72 10.46  8.73  9.31  9.55 11.22
## [12] 10.36 10.40 10.11  9.44 11.79 10.50  8.03 10.70  9.53  8.93  9.78
## [23]  8.97  9.27  9.37  8.31 10.84 10.15  8.86 11.25 10.43  9.70 10.90
## [34] 10.88 10.82 10.69 10.55  9.94  9.69  9.62
{% endhighlight %}



{% highlight r %}
knitr::kable(head(mtcars))
{% endhighlight %}



|                  |  mpg| cyl| disp|  hp| drat|   wt| qsec| vs| am| gear| carb|
|:-----------------|----:|---:|----:|---:|----:|----:|----:|--:|--:|----:|----:|
|Mazda RX4         | 21.0|   6|  160| 110| 3.90| 2.62| 16.5|  0|  1|    4|    4|
|Mazda RX4 Wag     | 21.0|   6|  160| 110| 3.90| 2.88| 17.0|  0|  1|    4|    4|
|Datsun 710        | 22.8|   4|  108|  93| 3.85| 2.32| 18.6|  1|  1|    4|    1|
|Hornet 4 Drive    | 21.4|   6|  258| 110| 3.08| 3.21| 19.4|  1|  0|    3|    1|
|Hornet Sportabout | 18.7|   8|  360| 175| 3.15| 3.44| 17.0|  0|  0|    3|    2|
|Valiant           | 18.1|   6|  225| 105| 2.76| 3.46| 20.2|  1|  0|    3|    1|



{% highlight r %}
par(mar = c(4,4,0.1,0.1))
plot(cars,pch=19,col="red")
{% endhighlight %}

![plot of chunk unnamed-chunk-1](https://dl.dropboxusercontent.com/u/59373967/jekyll/2016-09-17-second-post/unnamed-chunk-1-2.png)

{% highlight r %}
withMathJax(helpText('Dynamic output 1:  $$\\alpha^2$$'))
{% endhighlight %}



{% highlight text %}
## Error in eval(expr, envir, enclos): 沒有這個函數 "withMathJax"
{% endhighlight %}
