---
layout: page
permalink: /publications/
title: papers
description:
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
nav_order: 1
---
Another References:  <a href="https://scholar.google.com/citations?user=kEQgiVoAAAAJ" class="btn btn-sm z-depth-0" role="button"><i class="ai ai-google-scholar"></i>&nbsp;Google Scholar</a><a href="https://www.researchgate.net/profile/Young-Woon-Byeon" class="btn btn-sm z-depth-0" role="button"><i class="ai ai-researchgate"></i>&nbsp;ResearchGate</a><a href="https://orcid.org/0000-0003-2684-7720" class="btn btn-sm z-depth-0" role="button"><i class="ai ai-orcid"></i>&nbsp;ORCiD</a>

***†: equal contribution, *: corresponding author***

<!-- _pages/publications.md -->
<div class="publications">
  
  <h2 class="year">Soon</h2>
  {% bibliography -f papers -q @unpublished %}

  {% for y in page.years %}
    <h2 class="year">{{y}}</h2>
    {% bibliography -f papers -q @article[year={{y}}] %}
  {% endfor %}

</div>
