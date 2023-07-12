---
layout: page
permalink: /publications/
title: papers
description:
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
nav_order: 1
---
Another References: [<i class="fas fa-graduation-cap"></i> Google Scholar](https://scholar.google.com/citations?user={{ author.googlescholar }}) [<i class="fab fa-researchgate"></i> ResearchGate](https://www.researchgate.net/profile/{{ author.researchgate }}) [<i class="fab fa-orcid"></i> ORCID](http://orcid.org/{{ author.orcid }})

***†: equal contribution, *: corresponding author***

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
