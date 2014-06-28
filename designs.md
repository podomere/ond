---
layout: default
title: Designs Main Page
---

# Current Designs

<ul>
  {% for page in site.categories.designs %}
    <li>
      <a href="{{ page.url }}">{{ page.title }}</a>
    </li>
  {% endfor %}
</ul>
