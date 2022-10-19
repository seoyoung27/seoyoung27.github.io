---
layout: page
permalink: /publications/
title: Publications
description: <a>* indicates equal contribution.</a>
years: [2023, 2021]
poster_years: [2021]
domestic_years: [2019, 2017]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

## Conferences

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[kind=conference && year={{y}}]* %}
{% endfor %}

</div>

## Posters

<div class="publications">
{%- for y in page.poster_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[kind=poster, year={{y}}]* %}
{% endfor %}

</div>

## Domestic (Korean) Conferences

<div class="publications">
{%- for y in page.domestic_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[kind=domestic, year={{y}}]* %}
{% endfor %}

</div>