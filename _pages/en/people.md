---
layout: lab-en
permalink: /en/people/
translation: /people/
title: People
description: Faculty, staff, and students at VECTOR Lab.
lab_nav_order: 4
---

{% include lab-people-styles.liquid %}

{% for section in site.data.lab_people_en %}
<section class="people-section">
  <h2>{{ section.title | escape }}</h2>
  <div class="people-grid">
    {% for member in section.members %}
    <article class="people-card">
      <img src="{{ member.image | prepend: '/assets/img/people/' | relative_url }}" alt="{{ member.name | escape }}" loading="lazy">
      <div class="people-card__body">
        <h3>{{ member.name | escape }}</h3>
        <span class="role">{{ member.role | escape }}</span>
        <p>{{ member.summary | escape }}</p>
        {% if member.bio %}
        <details>
          <summary>Read bio</summary>
          <p>{{ member.bio | escape }}</p>
        </details>
        {% endif %}
      </div>
    </article>
    {% endfor %}
  </div>
</section>
{% endfor %}
