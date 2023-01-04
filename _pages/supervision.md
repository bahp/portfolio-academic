---
layout: page
permalink: /teaching/supervision/
title: supervision
description: work conducted by students grouped by year.
years: [2022, 2021, 2020]
nav: false
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f supervision -q @*[year={{y}}]* %}
{% endfor %}

</div>
