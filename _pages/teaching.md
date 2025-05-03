---
layout: page
title: Teaching
permalink: /teaching/
description:
nav: true
nav_order: 3
display_categories: [Courses]  # o las categorías que prefieras
horizontal: false
---

<!-- pages/teaching.md -->
<div class="teaching">
{% if site.enable_teaching_categories and page.display_categories %}
  <!-- Display categorized teaching items -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_items = site.teaching | where: "category", category %}
  {% assign sorted_items = categorized_items | sort: "priority" %}
  <!-- Generate cards for each teaching item -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for item in sorted_items %}
      {% include teaching_horizontal.liquid project=item %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for item in sorted_items %}
      {% include teaching.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display teaching items without categories -->

{% assign sorted_items = site.teaching | sort: "priority" %}

  <!-- Generate cards for each teaching item -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for item in sorted_items %}
      {% include teaching_horizontal.liquid project=item %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for item in sorted_items %}
      {% include teaching.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
