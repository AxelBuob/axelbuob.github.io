---
layout: default
title: Axel Buob
---
<div class="container intro txt-center">
  <h1>Hey..</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum consequuntur dicta consectetur nostrum! Quas suscipit commodi sed, minima, quisquam impedit minus dolorum. Saepe tempore magnam quae deleniti excepturi placeat obcaecati!</p>
  <button><a class="btn btn-big" href="/about">Lire la suite</a></button>
</div>

<div class="container flex column between wrap">
  {% for post in site.posts %}
  {% include _tags.md %}
  <article class="post">
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
<div class="container">
  <h1 class="txt-center">Get in touch..</h1>
  <div>
    {% include _form.md %}
  </div>
</div>
