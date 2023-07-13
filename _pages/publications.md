---
layout: page
permalink: /publications/
title: papers
description:
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
nav_order: 1
---
Another References:  [<i class="fas fa-graduation-cap"></i> Google Scholar](https://scholar.google.com/citations?user={{ author.googlescholar }}),   [<i class="fab fa-researchgate"></i> ResearchGate](https://www.researchgate.net/profile/{{ research_gate_profile }}),   [<i class="fab fa-orcid"></i> ORCID](https://orcid.org/{{ orcid_id }})

***†: equal contribution, *: corresponding author***

<!-- _pages/publications.md -->
<div class="unpublished">
  <h2 class="In Progress">{{y}}</h2>
  {% bibliography -f papers -q @unpublished* %}
</div>

<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @article*[year={{y}}]* %}
{% endfor %}
</div>
