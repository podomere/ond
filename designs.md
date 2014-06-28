---
layout: default
title: Main Design Index Page
---

# Current Designs


{{site.tags.designs}}


<ul>
{% assign sorted_pages = site.pages | sort:"name" %}
{% for node in sorted_pages %}
  <li><a href="{{node.url}}">{{node.title}}</a></li>
{% endfor %}
</ul>

<ul>
  {% for page in site.pages %}
    <li>
      <a href="{{ page.url }}">{{ page.title }}</a>{{page.excerpt}}
    </li>
  {% endfor %}
</ul>
