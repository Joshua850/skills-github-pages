---
layout: page
title: Blog
subtitle: Notes on engineering, automation, and staying sharp.
permalink: /blog/
---

<div class="post-grid">
{% for post in site.posts %}
  <article class="card">
    <a class="card__link" href="{{ post.url | relative_url }}">
      <time class="card__date" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d, %Y" }}</time>
      <h3 class="card__title">{{ post.title }}</h3>
      <p class="card__excerpt">{{ post.excerpt | strip_html | truncate: 140 }}</p>
      <span class="card__more">Read more &rarr;</span>
    </a>
  </article>
{% endfor %}
</div>
