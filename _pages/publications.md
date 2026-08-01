---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 2
---

<!-- Bibsearch Feature -->
{% include bib_search.liquid %}

<style>
  .publication-section-title {
    display: block !important;
    box-sizing: border-box !important;
    width: 100% !important;
    margin: 2.75rem 0 1rem !important;
    padding: 0 0 0.6rem !important;
    border: 0 !important;
    border-bottom: 1px solid
      var(--global-divider-color, #d8dee4) !important;
    font-size: 1.5rem !important;
    font-weight: 600 !important;
    line-height: 1.3 !important;
  }

  .publication-section-title--first {
    margin-top: 1.4rem !important;
  }

  .publication-section {
    margin: 0 !important;
    padding: 0 !important;
  }
</style>

<h2 class="publication-section-title publication-section-title--first">
  Preprints
</h2>

<div class="publications publication-section">
  {% bibliography --query @misc %}
</div>

<h2 class="publication-section-title">
  Conference Proceedings
</h2>

<div class="publications publication-section">
  {% bibliography --query @inproceedings %}
</div>

<h2 class="publication-section-title">
  Journal Articles
</h2>

<div class="publications publication-section">
  {% bibliography --query @article %}
</div>