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
  <h2 class="category"></h2>
  <!-- Generate cards for each project -->
    {% if page.horizontal -%}
    <div class="container">
      <div class="row row-cols-1">
      {%- for link in site.data.links.general %}
        {% include links_horizontal.html %}
      {% endfor %}
      {%- for link in site.data.links.books %}
        {% include links_horizontal.html %}
      {% endfor %}
      </div>
    </div>
    {%- else -%}
    <div class="grid">
      {%- for link in site.data.links.books %}
        {% include links.html %}
      {% endfor %}
    </div>
    {%- endif -%}
</div>
