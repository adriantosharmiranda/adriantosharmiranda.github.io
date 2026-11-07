---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

This page lists my published papers, preprints and theses. See also [Google Scholar](https://scholar.google.com/citations?user=98aWjBUAAAAJ), [ORCID](https://orcid.org/0009-0005-1767-8672) and [arXiv](https://arxiv.org/search/math?query=Miranda%2C+Adrian&searchtype=author).

{% include base_path %}

## Published papers

{% assign published = site.publications | where: "publication_type", "journal" | sort: "date" | reverse %}
{% for post in published %}
  {% include archive-single.html %}
{% endfor %}

## Preprints

{% assign preprints = site.publications | where: "publication_type", "preprint" | sort: "date" | reverse %}
{% for post in preprints %}
  {% include archive-single.html %}
{% endfor %}

## Theses

{% assign theses = site.publications | where: "publication_type", "thesis" | sort: "date" | reverse %}
{% for post in theses %}
  {% include archive-single.html %}
{% endfor %}
