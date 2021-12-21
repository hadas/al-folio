---
layout: page
permalink: /publications/
title: Publications
years: [2008, 2009, 2012, 2013, 2014, 2016, 2020]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

