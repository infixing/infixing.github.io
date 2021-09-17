---
layout: review
title: Tags
---
<h3>Reviews tagged with "{{ page.tag-name }}"</h3> 
{% for post in site.posts %} 
{% if post.tags contains page.tag-name %} 
{% include snippet.html %} 
{% endif %} 
{% endfor %}
