---
layout: default
title: Main Design Index Page
---

# Current Designs

<ul>
{% for page in site.pages %}	
  {% for tag in page.tags %}
    {% if tag == 'designs' %}
    	{% assign sorted_pages = sort:"name" %}
			{% for node in sorted_pages %}
				<li><a href="{{node.url}}">{{node.title}}</a> ({{node.description}})</li>
			{% endfor %}		
    {% endif %}
  {% endfor %}
{% endfor %}
</ul>

# License

* [http://ond.podome.re/LICENSE.html](http://ond.podome.re/LICENSE.html)

# Readme

* [http://ond.podome.re/README.html](http://ond.podome.re/README.html)
