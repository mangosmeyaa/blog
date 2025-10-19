---
layout: home   # <--- This tells you the layout file is likely _layouts/home.html
title: Home
---
<ul>
   {% for post in site.posts %}
     <li>
       <a href="{{ post.url | relative_url }}">{{
      post.title }} </a>
      </li>
     {% endfor %}
</ul>