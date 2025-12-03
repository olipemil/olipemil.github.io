---
layout: page
title: Visualizations
permalink: /visualizations/
description: Interactive visualizations and data explorations.
nav: true
nav_order: 4
display_categories: [materials, quantum, analysis]
horizontal: false
---

<!-- pages/visualizations.md -->
<div class="visualizations">
{% if site.enable_visualization_categories and page.display_categories %}
  <!-- Display categorized visualizations -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_visualizations = site.visualizations | where: "category", category %}
  {% assign sorted_visualizations = categorized_visualizations | sort: "importance" %}
  <!-- Generate cards for each visualization -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for visualization in sorted_visualizations %}
      {% include visualizations.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for visualization in sorted_visualizations %}
      {% include visualizations.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display visualizations without categories -->

{% assign sorted_visualizations = site.visualizations | sort: "importance" %}

  <!-- Generate cards for each visualization -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for visualization in sorted_visualizations %}
      {% include visualizations.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for visualization in sorted_visualizations %}
      {% include visualizations.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
