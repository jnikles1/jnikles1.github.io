---
layout: page
title: Resume
permalink: /resume/
---

{% for job in site.data.resume.jobs %}
  <h3>{{ job.name }}</h3>
  <h5>{{job.start-date}}-{{job.end-date}}</h5>
  <h4>{{ job.description }}</h4>
  <br>
{% endfor %}

