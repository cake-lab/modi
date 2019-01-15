---
layout: default
title: News
---

## Latest News

{% for post in site.posts %}
  * **[{{ post.date | date_to_string}} - {{ post.title }}]({{post.url}})**
    {{ post.excerpt }}
{% endfor %}
  