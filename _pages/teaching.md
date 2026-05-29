---
title: "Teaching & Mentoring"
layout: gridlay
sitemap: false
permalink: /teaching/
---

## Teaching & Mentoring

### Teaching

{% if site.data.courses and site.data.courses.size > 0 %}
{% for course in site.data.courses %}
<div class="section-card">
<h4>{{ course.name }}</h4>
<p><strong>Institution:</strong> {{ course.institution }} &nbsp;&nbsp; <strong>Term:</strong> {{ course.term }}</p>
<p>{{ course.desc }}</p>
</div>
{% endfor %}
{% else %}
<div class="section-card">
<p style="color: var(--text-secondary); font-style: italic;">Courses will be listed here as they are offered.</p>
</div>
{% endif %}

### Mentored Students & Interns

<div class="section-card">
{% if site.data.people %}
<ul>
{% for student in site.data.people %}
<li>{{ student.name }}, {{ student.location }} ({{ student.degree }}, {{ student.year }})</li>
{% endfor %}
</ul>
{% else %}
<p style="color: var(--text-secondary); font-style: italic;">Students and interns will be listed here.</p>
{% endif %}
</div>
