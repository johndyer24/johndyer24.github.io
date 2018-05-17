---
title: Projects
layout: experience
permalink: /projects/
---

{% for project in site.data.projects %}
  <div class="card" id="{{ project.id }}">
    <img class="card-pic" src="{{ project.image }}" alt="{{ project.title }}" height="200" width="200">
    <h2 class="card-title">{{ project.title }}</h2>
    <h3 class="card-subtitle">{{ project.subtitle }}</h3>
    <p class="card-description">{{ project.description | replace: '\', ''}}</p>
    {% if project.link %}
      <a class="card-button" href="{{ project.link }}">More Info</a>
    {% endif %}
  </div>
{% endfor %}
