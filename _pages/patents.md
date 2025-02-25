---
layout: default
permalink: /#patentid
title: patents
description: patents in reverse chronological order.
nav: true
nav_order: 2
---

<!-- _pages/patents.md -->
<div class="patents">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f patents -q @*[year={{y}}]* %}
{% endfor %}

</div>