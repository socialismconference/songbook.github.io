---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

{% assign sorted_pages = site.categories[songs] | sort: page.title %}
{% for page in sorted_pages %}
   
[{{ page.title }}]({{ site.baseurl }}{{ page.url }})
            
{% endfor %}
