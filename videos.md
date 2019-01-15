---
layout: default
title: Videos
---

## Videos
{% if site.videos.size == 0 %}
  * Currently there are no videos.  Please check back soon!
{% else %}
    {% for video in site.videos %}
  * [{{video.title}}]({{video.url}})
    {% endfor %}
{% endif %}