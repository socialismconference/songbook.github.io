---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

<p class="alphabet"><a href="#A">A</a>BCD<a href="#E">E</a>FGH<a href="#I">I</a>JKLMN<a href="#O">O</a>PQRST<a href="#U">U</a>VWXYZ</p>

{% assign sortedPages = site.pages | sort: page.title %}  
{% assign indexLetter = '' %}
{% for page in sortedPages %}  
   {% if page.url == '/' %}{% else %}
     {% assign firstLetter1 = page.title | capitalize  %}
     {% assign firstLetter = {{firstLetter1}} | truncate: 1, "" %}
     {% if {{firstLetter}} != {{indexLetter}} %}
       {% assign indexLetter1 = page.title | capitalize  %}
       {% assign indexLetter = {{indexLetter1}} | truncate: 1, "" %}

<h3 id="{{indexLetter}}"> {{ indexLetter }} </h3>

     {% endif %}

[{{ page.title }}]({{ site.baseurl }}{{ page.url }})
    
  {%endif%}  
{% endfor %}
