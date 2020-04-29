---
layout: default
title: Home
---

<main>
	{% for post in site.posts %}
		<div>
			<h1>{{ post.title }}</h1>
			<p><em>Date: {{ post.date | date_to_string }}</em></p>
			<p>{{ post.excerpt }}</p>
			<a href="{{ post.url }}">Read more</a>
		</div>
	{% endfor %}
</main>