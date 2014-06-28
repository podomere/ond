---
layout: default
title: Designs Main Page
---

# Current Designs

{{ site.pages }}

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
