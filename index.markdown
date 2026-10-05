---
layout: default
---

<h1 class="page-title">Projects</h1>
<p class="page-intro">{{ site.intro }}</p>

<div class="project-grid">
  {%- assign projects = site.projects | sort: "order" -%}
  {%- for project in projects -%}
    {% include project-card.html project=project %}
  {%- endfor -%}
</div>
