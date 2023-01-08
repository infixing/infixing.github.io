---
layout: tagpage
title: "Tag: YA"
tag: YA
---
{% for YA in site.tags %}
  <h3>{{ YA[0] }}</h3>
  <ul>
    {% for post in YA[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
