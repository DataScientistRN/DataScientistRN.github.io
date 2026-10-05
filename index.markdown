---
layout: default
---

<h1 class="page-heading">Projects</h1>

<div class="project-grid">
  {%- assign projects = site.projects | sort: "order" -%}
  {%- for project in projects -%}
    {% include project-card.html project=project %}
  {%- endfor -%}
</div>
