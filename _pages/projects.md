---
layout: page
title: projects
permalink: /projects/
description: A growing collection of Algotechniq projects
nav: true
nav_order: 2
display_categories: [work, fun]
horizontal: false
---

> Surface Defect Detection, Infrastructure Inspection

At Algotechniq, we specialize in AI-driven, real-time defect detection and infrastructure monitoring, leveraging deep learning algorithms and computer vision technologies to identify and classify defects such as cracks, corrosion, and deformities during manufacturing. This process not only enhances product quality and reduces waste but also ensures swift problem resolution.

> Traffic Safety, Building Security

In addition to these capabilities, Algotechniq automates routine infrastructure maintenance tasks using advanced machine learning. This allows for effective identification of issues in roads, tunnels, and buildings. Furthermore, our expertise in non-destructive testing enables us to decode complex data, significantly improving the accuracy of assessments.


<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
