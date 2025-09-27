---
layout: archive
title: "Data Analysis"
permalink: /data-analysis/
author_profile: true
---

{% include base_path %}

<img src="/images/Header-temporary.jpg" alt="Header Temporary">

These data analysis projects visualise open source environmental data and contain insights and details about how each project was developed. 

{% include base_path %}


{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}