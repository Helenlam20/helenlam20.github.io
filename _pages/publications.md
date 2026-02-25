---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2021, 2026]
nav: true
nav_order: 1
---

<div class="header">
</div>

<div class="publications">


<h1>Works in Progress</h1> 
{%- for y in page.years %}
  {% bibliography -f papers_working_paper -q @*[year={{y}}]* %}
{% endfor %}



<h1>Other Publications</h1>
{%- for y in page.years %}
  {% bibliography -f papers_published -q @*[year={{y}}]* %}
{% endfor %}


</div>

