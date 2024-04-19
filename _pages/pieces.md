---
layout: page
permalink: /pieces/
title: written pieces
description: Pieces of writing I worked on as a part of my courses or as an extension of my courses in form of a Star Variant.
years: [2023, 2022, 2021, 2020]
nav: true
nav_order: 2
---
<!-- _pages/pieces.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
