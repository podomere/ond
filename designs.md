---
layout: default
title: Main Design Index Page
---

# Current Designs


{{site.tags.designs}}

{% main_cat_page = site.pages.select { |p| p.name == /ond/} %}
{{main_cat_page}}


<ul>
{% assign sorted_pages = site.pages | sort:"name" %}
{% for node in sorted_pages %}
  <li><a href="{{node.url}}">{{node.title}}</a></li>
{% endfor %}
</ul>
