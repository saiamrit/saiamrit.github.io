---
layout: page-noheader
permalink: /publications/
title: tech blog
description: publications by categories in reversed chronological order. generated by jekyll-scholar.
years: []
nav: true
---
<div class="publications">
<iframe src="https://saiamrit.github.io/technical-blog/" style="width:800px; height:1024px;" frameborder="0"></iframe>

<!--- the original al-folio method, add years list to use --->
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %} 
</div>