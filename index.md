---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

Version 1

{% assign sortedPages = site.pages | sort: page.title %}  
{% assign indexLetter = '' %}
{% for page in sortedPages %}  
   {% if page.url == '/' %}{% else %}
     {% assign firstLetter = page.title | capitalize | truncate: 1 %}
     {% if firstLetter != indexLetter %}
       {% assign indexLetter = page.title | capitalize | truncate: 1 %}

### {{ firstLetter }}

     {% endif %}

[{{ page.title }}]({{ site.baseurl }}{{ page.url }})
    
  {%endif%}  
{% endfor %}

Version 1
