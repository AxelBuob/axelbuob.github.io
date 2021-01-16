---
permalink: /projects
layout: default
title: Projects
---
<div class="container">
    <h1>Les 12 travaux d'Hercule</h1>
</div>
<div class="container flex column between wrap">
  {% for post in site.posts %}
  {% include _tags.md %}
  <article class="sm-basis-1 md-basis-2 lg-basis-3 post">
    <ul class="post_tags">{{ tags }}</ul>
    <h2 class="post_title">{{ post.title }}</h2>
    <div class="post_excerpt">{{ post.excerpt }}</div>
    <p class="post_date">{{ post.date | date_to_string }}</p>
    <ul>
      <li><a href="{{ post.url }}">Live demo</a></li>
      <li><a href="{{ post.url }}">View code</a></li>
    </ul>
  </article>
  {% endfor %}
</div>
