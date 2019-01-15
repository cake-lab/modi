---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

## News
{% for post in site.posts limit: 10 %}
  * **{{ post.date | date_to_string}} - [{{ post.title }}]({{post.url | relative_url}})** - {{ post.excerpt | strip_html }}
{% endfor %}
{% if site.posts.size > 10 %}
  * [Click to see more news](news.html)
{% endif %}

{% assign sorted_publications = site.publications | sort: 'date_published'  %}
{% if sorted_publications.size > 0 %}
## Publications
{: .post-list-heading}

{% for publication in sorted_publications %}
* **[{{publication.title}}]({{publication.url | relative_url}})**. *{{publication.authors}}*. {{publication.journal}}.
{% endfor %}
{% endif %}

{% assign sorted_tutorials = site.tutorials | sort: 'date_published'  %}
{% if sorted_tutorials.size > 0 %}
## Tutorials
{% for tutorial in sorted_tutorials %}
* **[{{tutorial.title}}]({{tutorial.url | relative_url}})**. *{{tutorial.authors}}*. {{tutorial.journal}}.
{% endfor %}
{% endif %}

{% assign sorted_applications = site.applications | sort: 'date_published'  %}
{% if sorted_applications.size > 0 %}
## Applications
{% for application in sorted_applications %}
* **[{{application.title}}]({{application.url | relative_url}})**. *{{application.authors}}*. {{application.journal}}.
{% endfor %}
{% endif %}

{% assign sorted_videos = site.videos | sort: 'date_published'  %}
{% if sorted_videos.size > 0 %}
## Videos
{% for video in sorted_videos %}
* **[{{video.title}}]({{video.url | relative_url}})**. *{{video.authors}}*. {{video.journal}}.
{% endfor %}
{% endif %}