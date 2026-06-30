---
layout: page
title: Experience
subtitle: Where I&rsquo;ve worked and what I&rsquo;ve done.
permalink: /experience/
---

<div class="timeline">
{% for job in site.data.experience %}
  <div class="timeline__item">
    <div class="timeline__marker"></div>
    <div class="timeline__content">
      <div class="timeline__top">
        <h3 class="timeline__role">{{ job.role }}</h3>
        <span class="timeline__period">{{ job.period }}</span>
      </div>
      <p class="timeline__meta">{{ job.company }}{% if job.location %} · {{ job.location }}{% endif %}</p>
      {% if job.summary %}<p class="timeline__summary">{{ job.summary }}</p>{% endif %}
      {% if job.highlights %}
      <ul class="timeline__highlights">
        {% for h in job.highlights %}<li>{{ h }}</li>{% endfor %}
      </ul>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>

<h2 class="section-title" style="margin-top:48px;">Education</h2>
<div class="edu-list">
{% for edu in site.data.education %}
  <div class="edu-item">
    <div>
      <h3 class="edu-item__qual">{{ edu.qualification }}</h3>
      <p class="edu-item__inst">{{ edu.institution }}</p>
    </div>
    <span class="edu-item__period">{{ edu.period }}</span>
  </div>
{% endfor %}
</div>

{% if site.data.social.resume and site.data.social.resume != "" %}
<p class="page__cta"><a class="btn btn--primary" href="{{ site.data.social.resume | relative_url }}">Download full CV</a></p>
{% endif %}
