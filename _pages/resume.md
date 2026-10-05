---
layout: page
title: resume
permalink: /resume/
nav: true
nav_order: 3
---

{% assign cv = site.data.cv.cv %}

{{ cv.name }} · {{ cv.location }}

{{ cv.summary }}

## Education

{% for entry in cv.sections.Education %}
**{{ entry.institution }}**  
{{ entry.area }}
{% endfor %}

## Experience

{% for entry in cv.sections.Experience %}
**{{ entry.position }}** · {{ entry.company }} · {{ entry.date }}

{% if entry.summary %}{{ entry.summary }}{% endif %}
{% endfor %}

## Selected projects

{% for entry in cv.sections.Projects %}

### [{{ entry.name }}]({{ entry.url }})

{{ entry.summary }}
{% endfor %}
