---
layout: page
permalink: /publications/
title: selected publications
description: selected publications in reversed chronological order.
nav: true
nav_order: 4
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<p>This page contains selected publications. For the full list, visit my <a href="https://scholar.google.nl/citations?user=nB8yiM0AAAAJ&hl=en" target="_blank" rel="noopener noreferrer">Google Scholar profile</a>.</p>

<div class="publications">

{% bibliography --query @*[selected=true] %}

</div>
