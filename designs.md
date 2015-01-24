---
layout: default
title: Main Design Index Page
---

# Current Designs

<ul>

{% assign sorted_pages = site.pages | sort:"name" %}
{% for page in sorted_pages %}	
  {% for tag in page.tags %}
    {% tag where:"design" %}
		<li><a href="{{page.url}}">{{page.title}}</a> ({{page.description}})</li>	{% endif %}
  {% endfor %}
{% endfor %}
</ul>

# License

* [http://ond.podome.re/LICENSE.html](http://ond.podome.re/LICENSE.html)

# Readme

* [http://ond.podome.re/README.html](http://ond.podome.re/README.html)
