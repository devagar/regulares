---
layout: default
title: Aulas Regulares
---
<div class='post'>
    <div class='body'>
    {% for post in site.posts limit:1 %}
    	 <time datetime="{{ page.date | xmlschema }}">{{ page.date | date: "%d %b, %Y" }}</time>
      	<h2>{{ post.title }}</h2>
      	{{ post.content }}
    {% endfor %}
    </div>
</div>
<hr>
