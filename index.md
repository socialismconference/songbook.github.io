---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

Version 2

{% assign sortedPages = site.pages | sort: page.title %}  
{% assign indexLetter = '' %}
{% for page in sortedPages %}  
   {% if page.url == '/' %}{% else %}
     {% assign firstLetter = page.title | capitalize  %}
     {% if firstLetter != indexLetter %}
       {% assign indexLetter = page.title | capitalize  %}

<h3 id={{indexLetter}}> {{ indexLetter }} </h3>

     {% endif %}

[{{ page.title }}]({{ site.baseurl }}{{ page.url }})
    
  {%endif%}  
{% endfor %}

Version 2
