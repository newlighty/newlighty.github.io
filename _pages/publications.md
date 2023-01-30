---
layout: page
permalink: /publications/
title: انتشارات
description: انتشارات بر اساس دسته ها به ترتیب زمانی معکوس.
years: [1967, 1956, 1950, 1935, 1905]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
