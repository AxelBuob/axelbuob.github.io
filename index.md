---
layout: default
title: Axel Buob
---
<div>
	<h1>About</h1>
	<p><strong>Ce site blog est encore en construction. Merci de votre compréhension.</strong></p>
	<p><a href="/about">Read more</a></p>
</div>
<div>
	<h1>Latest posts</h1>
	{% for post in site.posts %}
	<article>
	  <h2>{{ post.title }}</h2>
	  <p>Date: {{ post.date | date_to_string }}</p>
	  {{ post.excerpt }}
	  <p><a href="{{ post.url }}">Read more</a></p>
	</article>
	{% endfor %}
</div>
<div>
	<h1>Contact</h1>
	<div>
		{% include form.md %}
	</div>
</div>
