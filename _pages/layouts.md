---
layout: default
title: Layouts
permalink: /layouts
---
<h1>Layouts</h1>
{% for post in site.categories.layouts %}
<div>
  <h2>{{ post.title }}</h2>
  <p>Date: {{ post.date | date_to_string }}</p>
  {{ post.excerpt }}
  <p><a href="{{ post.url }}">Read more</a></p>
</div>
{% endfor %}