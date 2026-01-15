---
title: "Cases"
permalink: /projects/
layout: single
author_profile: true
---

# Casos

Explore os cases que destacam decisões, trade-offs e impacto mensurável.

{% assign projects = site.data.projects | sort: 'order' %}

<div class="projects-grid" style="display:grid;gap:2rem;margin-top:2rem">
  {% for p in projects %}
  <article class="project-card" style="border:1px solid #e5e7eb;border-radius:8px;padding:1.5rem;background:#fff">
    <h3 style="margin-top:0"><a href="{{ site.baseurl }}{{ p.permalink }}" style="text-decoration:none;color:#1f2937">{{ p.title }}</a></h3>
    <p style="color:#6b7280;line-height:1.6">{{ p.short_blurb }}</p>
    <div style="display:flex;gap:1rem;align-items:center;margin-top:1rem">
      <span style="background:#f3f4f6;padding:0.25rem 0.75rem;border-radius:4px;font-size:0.9rem;font-weight:500">{{ p.key_metric }}</span>
      <span style="background:#e0f2fe;color:#0369a1;padding:0.25rem 0.75rem;border-radius:4px;font-size:0.85rem">{{ p.status }}</span>
    </div>
    <p style="margin-top:1rem"><a href="{{ site.baseurl }}{{ p.permalink }}" style="color:#2563eb;text-decoration:none;font-weight:500">Ver case →</a></p>
  </article>
  {% endfor %}
</div>
