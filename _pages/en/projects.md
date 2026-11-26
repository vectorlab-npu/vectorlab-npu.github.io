---
layout: lab-en
permalink: /en/projects/
translation: /projects/
title: Projects
description: Research projects led by or involving VECTOR Lab.
lab_nav_order: 2
---

<div class="projects">
  <div class="row row-cols-1 row-cols-md-3">
    {% assign english_projects = site.pages | where: 'lab_nav_parent', '/en/projects/' | sort: 'title' %}
    {% for project in english_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
