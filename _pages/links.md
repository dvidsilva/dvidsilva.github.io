---
layout: page
title: links
permalink: /links/
description: A growing collection of links to interesting content.
nav: true
nav_order: 1
display_categories: [work, fun]
horizontal: true
---

<!-- pages/links.md -->
<div class="projects">
  <!-- Display categorized links -->
  <h2 class="category">Books</h2>
  {%- for book in site.data.links.books %}
    <!-- Generate cards for each project -->
    {% if page.horizontal -%}
    <div class="container">
      <div class="row row-cols-2">
        {% include links_horizontal.html %}
      </div>
    </div>
    {%- else -%}
    <div class="grid">
      {% include links.html %}
    </div>
    {%- endif -%}
  {% endfor %}
</div>
