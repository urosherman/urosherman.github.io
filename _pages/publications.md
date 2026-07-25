---
layout: page
permalink: /publications/
title: research
description: for some older research, see also CV
years: [2026, 2025, 2023, 2021] 
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
