---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

This page lists my published papers, preprints and theses. Select a citation to read its abstract and follow links to the paper or thesis. See also [Google Scholar](https://scholar.google.com/citations?user=98aWjBUAAAAJ), [ORCID](https://orcid.org/0009-0005-1767-8672) and [arXiv](https://arxiv.org/search/math?query=Miranda%2C+Adrian&searchtype=author).

{% assign published = site.publications | where: "publication_type", "journal" | sort: "date" | reverse %}
{% assign preprints = site.publications | where: "publication_type", "preprint" | sort: "date" | reverse %}
{% assign theses = site.publications | where: "publication_type", "thesis" | sort: "date" | reverse %}

## Publications

<ol reversed="reversed" start="{{ published.size }}">
{% for post in published %}
  <li><a href="{{ post.url | relative_url }}">{{ post.citation | escape }}</a></li>
{% endfor %}
</ol>

## Preprints

<ol reversed="reversed" start="{{ preprints.size }}">
{% for post in preprints %}
  <li><a href="{{ post.url | relative_url }}">{{ post.citation | escape }}</a></li>
{% endfor %}
</ol>

## Theses

<ol reversed="reversed" start="{{ theses.size }}">
{% for post in theses %}
  <li><a href="{{ post.url | relative_url }}">{{ post.citation | escape }}</a></li>
{% endfor %}
</ol>
