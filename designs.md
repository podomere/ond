---
layout: default
title: Main Design Index Page
---

# Current Designs

<ul>
{% for page in site.pages %}	
{% for tag in page.tags %}
{% if tag == 'designs' %}
<li><a href="{{page.url}}">{{page.title}}</a> {{page.excerpt}}</li>
	{% endif %}
	{% endfor %}
	{% endfor %}
</ul>

# License

* [http://ond.podome.re/LICENSE.html](http://ond.podome.re/LICENSE.html)

# Readme

* [http://ond.podome.re/README.html](http://ond.podome.re/README.html)
