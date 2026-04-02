---
layout: page
permalink: /publications/
title: publications
description: Let there be light. 
years: [2026, 2025, 2024, 2023]
other_years: [2026, 2025, 2024, 2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h1>First / Co-first Author</h1>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<hr>

<h1>Other Contributions</h1>

{%- for y in page.other_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f others -q @*[year={{y}}]* %}
{% endfor %}

</div>
