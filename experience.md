---
title: Experience
layout: experience
permalink: /experience/
---
{% for experience in site.data.experience %}
  {% include card.html item=experience %}
{% endfor %}
