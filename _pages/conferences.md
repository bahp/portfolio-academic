---
layout: page
permalink: /publications/conferences/
title: conferences
description: conference publications grouped by year.
years: [2024, 2023, 2022, 2020, 2018, 2017, 2016, 2015, 2014]
nav: false
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>
