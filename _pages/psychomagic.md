---
layout: page
title: psychomagic
permalink: /psychomagic/
description: A short introduction to psychomagic.
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---

<!-- pages/psychomagic.md -->
<div class="projects">
  <!-- Display categorized links -->
  <h2 class="category">Books</h2>
  {%- for book in site.data.links.books %}
  <!-- Generate cards for each project -->
  <div class="grid">
    {% include links.html %}
  </div>
  {% endfor %}
</div>
