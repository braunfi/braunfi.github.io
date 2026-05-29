---
title: "Home"
layout: homelay
sitemap: false
permalink: /
---

<h2 class="home-hero">{{ site.name }}</h2>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
{% for item in site.data.research %}<a href="{{ site.url }}{{ site.baseurl }}/interests" class="chip">{{ item.title }}</a>
{% endfor %}</div>

<div class="callout" markdown="0">
<div class="callout-title"><i class="fa-solid fa-handshake callout-icon"></i> Open to Collaborations &amp; Internships</div>
<p>I am always happy to discuss research collaborations on video misinformation, responsible AI, or related topics. I also welcome prospective interns and students — see the <a href="https://media-bias-research.org/join-us/" target="_blank">Media Bias Group</a> and <a href="https://www.nii.ac.jp/en/about/international/mouresearch/" target="_blank">NII internship</a> pages, or <a href="mailto:{{ site.email }}">reach out directly</a>.</p>
</div>

<!--
<div class="callout callout-success" markdown="0">
<div class="callout-title"><i class="fa-solid fa-award callout-icon"></i> Award placeholder</div>
<p>Uncomment and update this block when you have an award or highlight to feature.</p>
</div>
-->

<!--
<div class="banner-frame" markdown="0">
<img src="{{ site.url }}{{ site.baseurl }}/images/banner.jpg" alt="Research banner" loading="lazy">
</div>
-->

### About me

I am a PhD student at the National Institute of Informatics (NII) and SOKENDAI in Tokyo, affiliated with the Media Bias Group.
My research focuses on video misinformation detection — developing AI systems that identify manipulated or decontextualized video content.
I work across the full detection pipeline, from analysing manipulation tactics and curating benchmark datasets to designing detection algorithms.
Beyond accuracy, I am interested in how detection systems communicate uncertainty to users and whether their decisions can be meaningfully explained.

### Publications

{% bibliography %}

<p><a href="{{ site.url }}{{ site.baseurl }}/publications">See all publications &rarr;</a></p>
