---
title: Table of Contents
layout: chapter
---

<ul>
{% assign sorted = (site.posts | sort: 'date') %}
{% for p in sorted %}
  {% if p.title != "Table of Contents" %}
  <li><a href="{{ site.baseurl }}{{ p.url }}">{{ p.title }}</a></li>
  {% endif %}
{% endfor %}
</ul>
