---
layout: page
permalink: /publications/
title: publications
description: The following is a list of my recent publications.
years: [2021]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
