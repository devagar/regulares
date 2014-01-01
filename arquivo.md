---
layout: default 
---
### Arquivo

**Aqui podem ser consultados todas as aulas e artigos publicados neste curso **

<div class="hfeed">
	{% for post in site.posts %}
	    <article class="hentry entry">
	    	<h3><time datetime="{{ post.date | xmlschema }}">{{ post.date | date: "%d-%m" }}</time>
	    	<a href="{{ base.url }}{{ post.url }}">{{ post.title }}</a></h3>
	    </article>
	{% endfor %}
</div>