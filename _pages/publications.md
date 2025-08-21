---
layout: page
permalink: /publications/
title: publications
description: 
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<h2 class="year">Publications</h2>
{% bibliography -f papers --query "type=article and not status=underreview and not status=workingpaper and not status=technicalreport" %}

<h2 class="year">Under Review</h2>
{% bibliography -f papers --query "@*[status=underreview]" %}

<h2 class="year">Working Papers</h2>
{% bibliography -f papers --query "@*[status=workingpaper]" %}

<h2 class="year">Technical Reports</h2>
{% bibliography -f papers --query "@*[status=technicalreport]" %}

{% bibliography %}

</div>

