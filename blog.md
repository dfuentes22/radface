---
layout: default
title: Blog
permalink: /blog/
---

<h2 class="page-title">Blog</h2>
<hr>
<div class="blog">
	
	{% for post in site.categories['Blog'] %}
	  <div class="blog-item">
		
		{% if post.image %}
			<a href="{{ site.baseurl }}{{ post.url }}"><img src="../img/{{ post.image }}" alt="..."></a>
		{% endif %}
		
		<h3>{{ post.title }}</h3>
		
		<p class="meta smaller">
		{% if post.author %}
			<span itemprop="author" itemscope itemtype="http://schema.org/Person"><span itemprop="name">{{ post.author }}</span></span> -
		{% endif %}
		<time datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">{{ post.date | date: "%b %-d, %Y" }}</time>
		</p>

		<p class="entry-summary">{{ post.excerpt }}</p>
		<hr>
		<p class="read-more"><a href="{{ site.baseurl }}{{ post.url }}">Read More</a></p>
	  </div>
	{% endfor %}	
</div>