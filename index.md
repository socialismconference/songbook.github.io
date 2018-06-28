---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

{% for page in site.pages %}
   
[{{ page.title }}]({{ site.baseurl }}{{ page.url }})
            
{% endfor %}
