---
layout: page
title: Projects
permalink: /projects/
description: 
nav: true
nav_order: 1
categories:
  - key: phd
    name: EAVISE
    display: horizontal
  - key: code
    name: Code & Data
    display: flexgrid
---

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.categories %}
  <!-- Display categorized projects -->
  {%- for category in page.categories %}
  <h2 class="category">{{ category.name }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category.key -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if category.display == "horizontal" -%}
  <div class="container">
    <div class="row row-cols-1">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {% elsif category.display == "flexgrid" -%}
  <div class="flexgrid">
    {%- for project in sorted_projects -%}
      {% include projects_flexgrid.html %}
    {%- endfor %}
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
