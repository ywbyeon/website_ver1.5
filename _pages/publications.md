---
layout: page
permalink: /publications/
title: papers
description:
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
nav_order: 1
---
You can also find my articles on: [<i class="fas fa-graduation-cap" aria-hidden="true"></i> Google Scholar](https://scholar.google.com/citations?user={{ author.googlescholar }}){: .btn .btn--primary .btn--googlescholar} [<i class="fab fa-researchgate" aria-hidden="true"></i> ResearchGate](https://www.researchgate.net/profile/{{ author.researchgate }}){: .btn .btn--primary .btn--researchgate} [<i class="fab fa-orcid" aria-hidden="true"></i> ORCID](http://orcid.org/{{ author.orcid }}){: .btn .btn--primary .btn--orcid}

***†: equal contribution, *: corresponding author***

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
