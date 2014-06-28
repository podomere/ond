---
layout: default
title: Main Design Index Page
---

# Current Designs


{{site.pages.tags.designs.size}}


<ul>
{% assign sorted_pages = site.pages | sort:"name" %}
{% for node in sorted_pages %}
  <li><a href="{{node.url}}">{{node.title}}</a></li>
{% endfor %}
</ul>
