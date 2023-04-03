---
layout: page
permalink: /publications/
title: publications
description: 
years: [2021, 2023]
nav: true
nav_order: 1
---

<div class="header">
</div>

<div class="publications">

<h1>working papers</h1>
{%- for y in page.years %}
  {% bibliography -f papers_working_paper -q @*[year={{y}}]* %}
{% endfor %}


<h1>other publications</h1>
{%- for y in page.years %}
  {% bibliography -f papers_published -q @*[year={{y}}]* %}
{% endfor %}


</div>

