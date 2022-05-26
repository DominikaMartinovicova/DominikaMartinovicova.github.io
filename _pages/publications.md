---
layout: page
permalink: /pieces/
title: Written pieces
description: Pieces of writing I worked on as a part of my courses or as an extension of my courses in form of a Star Variant.
years: [2022]
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
