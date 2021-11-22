--
layout: reviews
title: Young adult
--

{% for post in site.tags.YA %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
