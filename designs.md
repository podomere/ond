---
layout: default
title: Main Design Index Page
---

# Current Designs


{{site.pages.tags}}

Post Tags
{{post.tags}}


<ul>
{% assign sorted_pages = site.pages | sort:"name" %}
{% for node in sorted_pages %}
  <li><a href="{{node.url}}">{{node.title}}</a> {{node.tags}}</li>
{% endfor %}
</ul>

<ul>
{% for page in site.pages %}	
{% for tag in page.tags %}
{% if tag == 'designs' %}
<li><a href="{{page.url}}">{{page.title}}</a> {{page.tags}}</li>
	{% endif %}
	{% endfor %}
	{% endfor %}
</ul>
