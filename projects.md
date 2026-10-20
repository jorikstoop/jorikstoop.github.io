---
layout: page
title: Projects
permalink: /projects/
---

<!-- Create boxes for each project -->
{%- if site.projects.size > 0 -%}
  <div class="project-list">
    {%- for project in site.projects -%}
    {%- if project.published -%}
      <div class="project-container">
        {% if project.external_url %}
          <a href="{{ project.external_url }}" class="project-link" target="_blank">
        {% else %}
          <a href="{{ project.url }}" class="project-link">
        {% endif %}
        <div class = "project-image-container"><img src="{{ project.cover_img }}" alt="Cover Image"></div>
        <div class="project-title-container">{{project.title}}</div>
        </a>
      </div>
    {%- endif -%}
    {%- endfor -%}
  </div>
{%- endif -%}