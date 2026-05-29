---
title: "Resources"
layout: gridlay
sitemap: false
permalink: /resources/
---

## Resources

{% if site.data.resources and site.data.resources.size > 0 %}
<div class="research-grid">
{% for item in site.data.resources %}
<div class="research-card">
{% if item.image %}<img src="{{ site.url }}{{ site.baseurl }}/images/{{ item.image }}" class="research-thumb" alt="{{ item.title }}" loading="lazy">{% endif %}
<div class="research-body">
{% if item.type or item.year %}<p style="margin: 0 0 var(--space-2); font-size: 0.75rem; color: var(--text-muted); text-transform: uppercase; letter-spacing: 0.05em;">{% if item.type %}{{ item.type }}{% endif %}{% if item.type and item.year %} &middot; {% endif %}{% if item.year %}{{ item.year }}{% endif %}</p>{% endif %}
<h4 class="research-title">{{ item.title }}</h4>
<p class="research-desc">{{ item.desc }}</p>
{% if item.url %}<a href="{{ item.url }}" target="_blank" class="btn-pill btn-website" style="margin-top: var(--space-2);">Explore &rarr;</a>{% endif %}
</div>
</div>
{% endfor %}
</div>
{% else %}
<div class="section-card">
<p style="color: var(--text-secondary);">No resources yet — check back soon.</p>
</div>
{% endif %}
