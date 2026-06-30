---
layout: page
title: About
subtitle: Full stack engineer focused on production, cloud-native systems.
permalink: /about/
---

I&rsquo;m a full stack software engineer based in {{ site.data.social.location }}, with 4+ years
of experience building and operating large-scale, production IoT applications on cloud-native
platforms. I work end-to-end — from designing and building backend services to deploying,
monitoring and keeping them reliable in production.

At **Davra** I build backend services in TypeScript and Node.js for real-time data ingestion,
processing and visualisation, ship them as containerised microservices on Kubernetes and AWS,
and build the customer-facing applications on top with Vue 3. I came into the team as a QA
engineer — designing automated test frameworks with Playwright and building observability with
Prometheus and Grafana — which gave me a strong, first-hand understanding of production failure
modes and what it actually takes to keep cloud-native systems reliable.

Outside of work I build things I&rsquo;d want to use myself. My main project, **TCG Swap**, is a
full-stack trading card platform with 130,000+ cards and real users — covering collaborative deck
building, peer-to-peer trading, camera-based card scanning with OCR, and live multiplayer game
tools. I like projects that force me across the whole stack, from the database up to the camera.

I&rsquo;m an Irish citizen with EU work authorization (no sponsorship required) and I&rsquo;m open
to new opportunities.

## Skills

<div class="skills">
{% for group in site.data.skills %}
  <div class="skills__group">
    <h3 class="skills__heading">{{ group.category }}</h3>
    <ul class="tag-list">
      {% for item in group.items %}<li class="tag">{{ item }}</li>{% endfor %}
    </ul>
  </div>
{% endfor %}
</div>

## Get in touch

The best way to reach me is by [email](mailto:{{ site.data.social.email }}){% if site.data.social.github and site.data.social.github != "" %}, or find me on [GitHub]({{ site.data.social.github }}){% endif %}{% if site.data.social.linkedin and site.data.social.linkedin != "" %} and [LinkedIn]({{ site.data.social.linkedin }}){% endif %}.
