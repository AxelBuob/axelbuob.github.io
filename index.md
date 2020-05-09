---
layout: default
title: Axel Buob
---
<div class="container txt-center">
	<h1>Hey..</h1>
	<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum consequuntur dicta consectetur nostrum! Quas suscipit commodi sed, minima, quisquam impedit minus dolorum. Saepe tempore magnam quae deleniti excepturi placeat obcaecati!</p>
	<button><a class="btn btn-big" href="/about">Read more</a></button>
</div>

<div class="container flex column between wrap">
	{% for post in site.posts %}
		{% assign tags = post.tags | join:' | ' %}
	<article class="sm-basis-1 md-basis-2 lg-basis-3 post">
		<h2>{{ post.title }}</h2>
		<p>{{ post.date | date_to_string }}</p>
		<p>{{ tags }}</p>
		<div>{{ post.excerpt }}</div>
		<button><a class="btn" href="{{ post.url }}">Read more</a></button>
	</article>
	{% endfor %}
</div>


<!-- <div class="container">
	<h1 class="txt-center">Get in touch..</h1>
	<div>
		{% include form.md %}
	</div>
</div> -->
