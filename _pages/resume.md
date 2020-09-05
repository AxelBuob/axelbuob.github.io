---
permalink: /resume
layout: default
title: Curriculum vitae
---
<div class="container">
  <h1>Le parcours du combattant</h1>
  <h2>Compétences</h2>
  <ul>
  {% for skill in site.data.resume.skills %}
    <li>{{ skill.name }}</li>
  {% endfor %}
  </ul>
  <h2>Expériences</h2>
  <ul>
  {% for experience in site.data.resume.experiences %}
    <li>
      {{ experience.date }} // {{ experience.name }}
      <br>
      {{ experience.company }} // {{ experience.where }}
    </li>
  {% endfor %}
  </ul>
  <h2>Formation</h2>
  <ul>
  {% for formation in site.data.resume.formations %}
    <li>
    {{ formation.date }} // {{ formation.name }}
    <br>
    {{ formation.school }} // {{ formation.where }}
    </li>
  {% endfor %}
  </ul>
  <h2>Langues</h2>
    <ul>
    {% for language in site.data.resume.languages %}
      <li>{{ language.name }} ({{language.level}})</li>
    {% endfor %}
    </ul>
  <h2>Intérêts</h2>
  <ul>
    {% for interest in site.data.resume.interests %}
      <li>{{ interest.name }}</li>
    {% endfor %}
  </ul>
</div>
