---
layout: default
title: Main Design Index Page
description: Summary Design Page
tags: designlist
type: design
author: Donal O Duibhir, 2014, @irldexter @donalod

---

# Current Designs

<ul>

{% assign sorted_pages = site.pages | sort:"name" %}
{% for page in sorted_pages %}	
  {% for tag in page.tags %}
    {% if tag == "design" %}
		<li><a href="{{page.url}}">{{page.title}}</a> ({{page.description}})</li>	{% endif %}
  {% endfor %}
{% endfor %}
</ul>

# License

* [https://opennetworkdesign.com/LICENSE.html](https://opennetworkdesign.com/LICENSE.html)

# Readme

* [https://opennetworkdesign.com/README.html](https://opennetworkdesign.com/README.html)
