---
title: Red Hootenanny Song Index
permalink: /
---
## Songs for Socialism 2018

**Raise Your Voice with Us  
Thursday, July 5 at 9:30PM  
In the lobby outside the Haymarket Books room**

> Organized by the totally **un-**official S18 Red Hootenanny Committee

<div class="alphabet">&nbsp;&thinsp;</div>

[#](#)
[A](#A)
[B](#B)
[C](#C)
[D](#D)
[E](#E)
[F](#F)
[G](#G)
[H](#H)
[I](#I)
[J](#J)
[K](#K)
[L](#L)
[M](#M)
[N](#N)
[O](#O)
[P](#P)
[Q](#Q)
[R](#R)
[S](#S)
[T](#T)
[U](#U)
[V](#V)
[W](#W)
[X](#X)
[Y](#Y)
[Z](#Z)

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
