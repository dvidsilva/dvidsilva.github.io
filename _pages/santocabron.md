---
layout: landing
title: santo cabron
permalink: /santocabron/
og_image: /assets/img/santocabron-horizontal.png
description: 'Santo Cabron is an alterlatinx art collective in NY. Support their brujas and warlocks create participatory experiences. #alterlatinx #horneylife #santocabron'
nav: false
horizontal: true
---
## Links in bio

<div class="projects">
  <!-- Display categorized links -->
  <h2 class="category"></h2>
  <!-- Generate cards for each project -->
    {% if page.horizontal -%}
    <div class="container">
      <div class="row row-cols-1">
      {%- for link in site.data.links.santocabron %}
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
  <img src="/assets/img/santocabron-horizontal.png" alt="santo cabron" style="max-width: 100%">
</div>

