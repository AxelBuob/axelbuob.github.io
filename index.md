---
layout: default
title: Axel Buob
---
<div class="container">
	<h1 class="txt-center">Hey..</h1>
	<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum consequuntur dicta consectetur nostrum! Quas suscipit commodi sed, minima, quisquam impedit minus dolorum. Saepe tempore magnam quae deleniti excepturi placeat obcaecati!</p>
	<button><a href="/about">Read more</a></button>
</div>

<div class="container flex column between wrap">
	{% for post in site.posts %}
	<article class="w30">
		<h2>{{ post.title }}</h2>
		<p>Date: {{ post.date | date_to_string }}</p>
		<div class="txt-justify">{{ post.excerpt }}</div>
		<button><a href="{{ post.url }}">Read more</a></button>
	</article>
	{% endfor %}
</div>


<div class="container">
	<h1 class="txt-center">Get in touch..</h1>
	<div>
		{% include form.md %}
	</div>
</div>
