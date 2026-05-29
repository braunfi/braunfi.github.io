---
title: "Interests"
layout: gridlay
sitemap: false
permalink: /interests/
---

## Research Interests

<div class="research-grid">
{% for item in site.data.research %}
<div class="research-card">
{% if item.image %}<img src="{{ site.url }}{{ site.baseurl }}/images/{{ item.image }}" class="research-thumb" alt="{{ item.title }}" loading="lazy">{% endif %}
<div class="research-body">
<h4 class="research-title">{{ item.title }}</h4>
<p class="research-desc">{{ item.desc }}</p>
</div>
</div>
{% endfor %}
</div>
