---
layout: review
title: Tags
---
{% assign category = site.tags | where: "slug", post.category %}
{% assign category = category[0] %}
{% if category %}
    {% capture category_content %}<a class="label" href="{{ category.url }}">{{ category.name }}</a>{% endcapture %}
{% endif %}
