---
layout: page
title: Interstellar  
tagline: Extracting thoughts...
---
{% include JB/setup %}


## Post Lists ###

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


----------

### References ###
 - Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html) for more info.
 - Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)
 - If you'd like to be added as a contributor, [please fork](http://github.com/plusjade/jekyll-bootstrap)!


