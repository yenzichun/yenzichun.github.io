---
layout: post
title:  dashboard test
date: "2016-09-22 23:21:24"
published: true
tags: [example1, example2]
output:
  flexdashboard::flex_dashboard:
    orientation: columns
    source_code: embed
---



{% highlight text %}
## Error in loadNamespace(name): there is no package called 'webshot'
{% endhighlight %}


{% highlight text %}
## Error in loadNamespace(name): there is no package called 'webshot'
{% endhighlight %}



<!--
Column {.tabset .tabset-fade}
---

### Chart A


{% highlight r %}
l1 <- city_group_count %>% filter(yy==2007)
l2 <- city_group_count %>% filter(yy==2008)
l3 <- city_group_count %>% filter(yy==2009)
l4 <- city_group_count %>% filter(yy==2010)
l5 <- city_group_count %>% filter(yy==2011)
l6 <- city_group_count %>% filter(yy==2012)
l7 <- city_group_count %>% filter(yy==2013)
citylist <- levels(as.factor(city_group_count$city2))
yrlist <- levels(as.factor(city_group_count$yy))


y <- city_group_count %>% spread(.,city2,count)



highchart() %>%
  hc_chart(type = "column") %>%
  hc_title(text = "stacked column chart") %>%
  hc_xAxis( categories = citylist) %>%
  hc_yAxis( stackLabels = list( enabled = TRUE)) %>%
  hc_plotOptions( column = list( stacking = "normal")) %>%
  hc_add_series(name="2013",data = l7$count) %>%
  hc_add_series(name="2012",data = l6$count) %>%
  hc_add_series(name="2011",data = l5$count) %>%
  hc_add_series(name="2010",data = l4$count) %>%
  hc_add_series(name="2009",data = l3$count) %>%
  hc_add_series(name="2008",data = l2$count) %>%
  hc_add_series(name="2007",data = l1$count)
{% endhighlight %}



{% highlight text %}
## Error in loadNamespace(name): there is no package called 'webshot'
{% endhighlight %}

### Chart B


{% highlight r %}
citylist <- levels(as.factor(city_group_count$city2))
yrlist <- levels(as.factor(city_group_count$yy))
y <- city_group_count %>% spread(.,city2,count)

highchart() %>%
  hc_chart(type = "column") %>%
  hc_title(text = "stacked column chart") %>%
  hc_xAxis( categories = yrlist) %>%
  hc_yAxis( stackLabels = list( enabled = TRUE)) %>%
  hc_plotOptions( column = list( stacking = "normal")) %>%
  hc_add_series(name=citylist[1],data = y$台中市) %>%
  hc_add_series(name=citylist[2],data = y$台北市) %>%
  hc_add_series(name=citylist[3],data = y$台東縣) %>%
  hc_add_series(name=citylist[4],data = y$台南市) %>%
  hc_add_series(name=citylist[5],data = y$宜蘭縣) %>%
  hc_add_series(name=citylist[6],data = y$花蓮縣) %>%
  hc_add_series(name=citylist[7],data = y$金門縣) %>%
  hc_add_series(name=citylist[8],data = y$南投縣) %>%
  hc_add_series(name=citylist[9],data = y$屏東縣) %>%
  hc_add_series(name=citylist[10],data = y$苗栗縣) %>%
  hc_add_series(name=citylist[11],data = y$桃園縣) %>%
  hc_add_series(name=citylist[12],data = y$高雄市) %>%
  hc_add_series(name=citylist[13],data = y$基隆市) %>%
  hc_add_series(name=citylist[14],data = y$連江縣) %>%
  hc_add_series(name=citylist[15],data = y$雲林縣) %>%
  hc_add_series(name=citylist[16],data = y$新北市) %>%
  hc_add_series(name=citylist[17],data = y$新竹市) %>%
  hc_add_series(name=citylist[18],data = y$新竹縣) %>%
  hc_add_series(name=citylist[19],data = y$嘉義市) %>%
  hc_add_series(name=citylist[20],data = y$嘉義縣) %>%
  hc_add_series(name=citylist[21],data = y$彰化縣) %>%
  hc_add_series(name=citylist[22],data = y$澎湖縣)
{% endhighlight %}



{% highlight text %}
## Error in loadNamespace(name): there is no package called 'webshot'
{% endhighlight %}
-->
