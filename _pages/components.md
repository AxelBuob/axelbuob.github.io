---
layout: default
title: Components
permalink: /components
---
<h1>Components</h1>
{% for post in site.categories.components %}
<div>
  <h2>{{ post.title }}</h2>
  <p>Date: {{ post.date | date_to_string }}</p>
  {{ post.excerpt }}
  <p><a href="{{ post.url }}">Read more</a></p>
</div>
{% endfor %}