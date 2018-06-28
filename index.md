---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

{% for post in site.posts %}
   
[{{ post.title }}]({{ site.baseurl }}{{ post.url }})
            
{% endfor %}
