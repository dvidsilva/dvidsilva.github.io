---
layout: page
title: services
permalink: /services/
description: A brief description of my offerings.
nav: true
nav_order: 9
display_categories: [work, fun]
horizontal: true
---

```
@TODO: missing data interpolation
```
<!-- pages/links.md -->
<div class="projects">
  <!-- Display categorized links -->
  <h2 class="category">Tech</h2>
  <!-- Generate cards for each project -->
    {% if page.horizontal -%}
    <div class="container">
      <div class="row row-cols-1">
      {%- for link in site.data.services.tech %}
        {% include links_horizontal.html %}
      {% endfor %}
      </div>
    </div>
    {%- else -%}
    <div class="grid">
      {%- for link in site.data.services.tech %}
        {% include links.html %}
      {% endfor %}
    </div>
    {%- endif -%}


  <h2 class="category">Community</h2>
  <!-- Generate cards for each project -->
    {% if page.horizontal -%}
    <div class="container">
      <div class="row row-cols-1">
      {%- for link in site.data.services.community %}
        {% include links_horizontal.html %}
      {% endfor %}
      </div>
    </div>
    {%- else -%}
    <div class="grid">
      {%- for link in site.data.services.community %}
        {% include links.html %}
      {% endfor %}
    </div>
    {%- endif -%}
</div>
