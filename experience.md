---
title: Experience
layout: experience
permalink: /experience/
---
{% for experience in site.data.experience %}
  <div class="card" id="{{ experience.id }}">
    <img class="card-pic" src="{{ experience.image }}" alt="{{ experience.title }}" height="200" width="200">
    <h2 class="card-title">{{ experience.title }}</h2>
    <h3 class="card-subtitle">{{ experience.subtitle }}</h3>
    <p class="card-description">{{ experience.description | replace: '\', ''}}</p>
    {% if experience.link %}
      <a class="card-button" href="{{ experience.link }}">More Info</a>
    {% endif %}
  </div>
{% endfor %}
