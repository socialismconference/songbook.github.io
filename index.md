---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

{% assign sorted_posts = site.post | sort: post.title %}
{% for post in sorted_posts %}
   
[{{ post.title }}]({{ site.baseurl }}{{ post.url }})
            
{% endfor %}
