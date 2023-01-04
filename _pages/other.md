---
layout: page
permalink: /publications/other/
title: other publications
description: other type of publications grouped by year.
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014]
nav: false
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f other -q @*[year={{y}}]* %}
{% endfor %}

</div>