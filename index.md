---
layout: default
title: mZero
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

### Artigos Publicados

<div class="hfeed">
	{% for post in site.posts %}
	   <article class="hentry entry">
	    	<p><time datetime="{{ post.date | xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
	    	<a href="{{ post.url }}">{{ post.title }}</a></p>
	    </article>
	{% endfor %}
</div>
