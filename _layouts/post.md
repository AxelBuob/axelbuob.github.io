---
layout: default
---
<main>
	<h1>{{ page.title}}</h1>
	<p><em>Date: {{ page.date | date_to_string }}</em></p>
	<p>{{ page.content }}</p>
</main>