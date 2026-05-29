---
title: "Software"
layout: gridlay
sitemap: false
permalink: /software/
---

## Software

{% if site.data.software and site.data.software.size > 0 %}
{% for project in site.data.software %}
<div class="section-card">
<h4><a href="https://github.com/{{ project.repo }}" target="_blank">{{ project.name }}</a></h4>
<div class="pub-actions" style="margin-bottom: var(--space-3);">
{% if project.website %}<a href="{{ project.website }}" target="_blank" class="btn-pill btn-website">Website</a>{% endif %}
<a href="https://github.com/{{ project.repo }}" target="_blank" class="btn-pill btn-git">Git</a>
</div>
<p><strong>Authors:</strong> <em>{{ project.authors }}</em></p>
<p>{{ project.desc }}</p>
</div>
{% endfor %}
{% else %}
<div class="section-card">
<p style="color: var(--text-secondary); font-style: italic;">Open-source tools are in preparation and will be listed here soon. In the meantime, you can find my projects on <a href="{{ site.links.github }}">GitHub</a>.</p>
</div>
{% endif %}
