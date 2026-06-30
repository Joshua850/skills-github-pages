---
layout: page
title: Projects
subtitle: Things I&rsquo;ve built — from production platforms to front-end experiments.
permalink: /projects/
---

<ul class="project-list">
{% for project in site.data.projects %}
  <li class="project-row">
    <div class="project-row__head">
      <h3 class="project-row__name">{{ project.name }}</h3>
      {% if project.demo and project.demo != "" %}<a class="project-row__link" href="{{ project.demo }}" target="_blank" rel="noopener">Live demo ↗</a>{% endif %}
    </div>
    <p class="project-row__desc">{{ project.description }}</p>
    {% if project.tags %}<ul class="tag-list tag-list--sm">{% for t in project.tags %}<li class="tag">{{ t }}</li>{% endfor %}</ul>{% endif %}
  </li>
{% endfor %}
</ul>
