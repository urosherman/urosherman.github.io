---
layout: page
permalink: /publications/
title: research
description: for some older research see also CV
years: [2023, 2022, 2021, 2016] 
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
