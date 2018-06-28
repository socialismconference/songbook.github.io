---
title: Songs to Sing at Socialism
description: A listing of lyrics for songs at the patio sing-along
permalink: /
---
## Songs for Socialism 2018

   {% assign sorted_pages = site.pages | sort: post.title %}
   {% for page in sorted_pages %}
    <p>
          <a href="{{ site.baseurl }}{{ page.url }}">
            {{ page.title }}
          </a>
    </p>   {% endfor %} </ul>
