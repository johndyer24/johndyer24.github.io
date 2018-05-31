---
title: Projects
layout: experience
permalink: /projects/
---

{% for project in site.data.projects %}
  {% include card.html item=project %}
{% endfor %}
