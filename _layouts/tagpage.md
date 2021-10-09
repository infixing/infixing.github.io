---
layout: default
---
<div class="post">
Tag: {{ page.tag }}
<ul>
{% for post in site.tags[page.tag] %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date_to_string }})<br>
    {{ post.description }}
  </li>
{% endfor %}
</ul>
</div>
<hr>
