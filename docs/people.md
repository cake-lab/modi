---
layout: default
title: People
---

<!---
Cake Lab is based at Worcester Polytechnic Institute
--->


{% assign pi_list = site.authors | where:"role.short","PI" %}
{% assign phd_list = site.authors | where:"role.short","PhD" %}


## Principal Investigators
{% for author in pi_list %}
  * [{{author.name}}]({{author.url}}), {{author.role.title}} @ {{author.organizaton_short}} 
{% endfor %}

## Students
{% for author in phd_list %}
  * [{{author.name}}]({{author.url}}), {{author.role.title}} @ {{author.organizaton_short}}  
{% endfor %}

