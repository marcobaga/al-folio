---
layout: page
permalink: /publications/
title: publications
description: A list of published works in which I was involved.
years: [2023, 2022, 2021]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
