---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

{% assign sortedPosts = site.post | sort: 'title' %}
{% for post in sortedPosts %}
   
[{{ post.title }}]({{ site.baseurl }}{{ post.url }})
            
{% endfor %}
