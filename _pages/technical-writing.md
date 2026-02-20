---
layout: page
title: Technical Writing
permalink: /work/technical-writing/
description: A portfolio of my technical writing work — samples, case studies, and documentation projects.
nav: false
---

## Writing Samples

A selection of documentation, guides, and reference material I've created across industries.

{% assign writing_samples = site.projects | where: "category", "writing-sample" %}
{% for project in writing_samples %}
  {% include projects.liquid project=project %}
{% endfor %}

---

## Case Studies

Deep dives into documentation challenges I've solved — the problem, my approach, and the outcome.

{% assign case_studies = site.projects | where: "category", "case-study" %}
{% for project in case_studies %}
  {% include projects.liquid project=project %}
{% endfor %}