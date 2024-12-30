---
layout: page
permalink: /teaching/
title: teaching
description: Materials for courses you taught. Replace this text with your description.
nav: true
nav_order: 6
---
<!-- pages/teachings.md -->
<div class="teachings">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized teachings -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_teachings = site.teachings | where: "category", category %}
  {% assign sorted_teachings = categorized_teachings | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_teachings %}
      {% include teachings_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_teachings %}
      {% include teachings.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display teachings without categories -->

{% assign sorted_teachings = site.teachings | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_teachings %}
      {% include teachings_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_teachings %}
      {% include teachings.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>