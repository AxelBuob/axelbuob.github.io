---
layout: default
title: Typography
permalink: /typography
---
<h1>Typography</h1>
{% for post in site.categories.typography %}
<div>
  <h2>{{ post.title }}</h2>
  <p>Date: {{ post.date | date_to_string }}</p>
  {{ post.excerpt }}
  <p><a href="{{ post.url }}">Read more</a></p>
</div>
{% endfor %}

