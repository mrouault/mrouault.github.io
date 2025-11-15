---
permalink: "/research/"
layout: single
classes: wide
author_profile: true
title: "Research"
#toc: true
#toc_label: "Publications"
#toc_sticky: true
---

My publications can be found on <a href="https://scholar.google.com/citations?hl=en&user=sG650W8AAAAJ">Google scholar</a> or <a href="https://arxiv.org/a/0009-0001-1299-7587">arXiv</a>.

<!-- Go to _config.yml file and fill the corresponding fields author.academic_profiles.xxxx-->


<!-- See also https://github.com/inukshuk/jekyll-scholar to customize your references -->

<!-- Preprints -->
{% capture counter_preprints %}{% bibliography_count --query @unpublished %}{% endcapture %}
{% if counter_preprints != "0" %}

## Preprints

  {% bibliography --query @unpublished %}
{% endif %}

<!-- Journal articles-->
{% capture counter_book %}{% bibliography_count --query @book %}{% endcapture %}
{% if counter_book != "0" %}

## Books

  {% bibliography --query @book %}
{% endif %}

<!-- Journal articles-->
{% capture counter_article %}{% bibliography_count --query @article %}{% endcapture %}
{% if counter_article != "0" %}

## Journal articles

  {% bibliography --query @article %}
{% endif %}

<!-- Conference papers -->
{% capture counter_inproceedings %}{% bibliography_count --query @inproceedings %}{% endcapture %}
{% if counter_inproceedings != "0" %}

## Conference papers

  {% bibliography --query @inproceedings %}
{% endif %}

<!-- Workshop papers -->
{% capture counter_workshop %}{% bibliography_count --query @misc[keywords=workshop] %}{% endcapture %}
{% if counter_workshop != "0" %}

## Workshop papers

  {% bibliography --query @misc[keywords=workshop] %}
{% endif %}

<!-- Thesis -->
{% capture counter_thesis %}{% bibliography_count --query @thesis %}{% endcapture %}
{% if counter_thesis != "0" %}

## Thesis

  {% bibliography --query @thesis %}
{% endif %}

<!-- Popularization -->
{% capture counter_popularization %}{% bibliography_count --query @misc[keywords=popularization] %}{% endcapture %}
{% if counter_popularization != "0" %}

## Popularization

  {% bibliography --query @misc[keywords=popularization] %}
{% endif %}
