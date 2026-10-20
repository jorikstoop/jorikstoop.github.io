---
layout: page
title: Hobbies
permalink: /hobbies/
---

<!-- Create boxes for each hobby -->
{%- if site.hobbies.size > 0 -%}
  <div class="project-list">
    {%- for hobby in site.hobbies -%}
    {%- if hobby.published -%}
      <div class="project-container">
        <a href="{{ hobby.url }}" class = "project-link">
        <div class = "project-image-container"><img src="{{ hobby.cover_img }}" alt="Cover Image"></div>
        <div class="project-title-container">{{hobby.title}}</div>
        </a>
      </div>
    {%- endif -%}
    {%- endfor -%}
  </div>
{%- endif -%}