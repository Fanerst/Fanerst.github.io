---
title: "Talks"
layout: gridlay
sitemap: false
permalink: /talks/
---

## Talks

{% if site.data.talks.size > 0 %}
<div class="section-card" markdown="0">
<div class="news-timeline">
{% for talk in site.data.talks %}
<div class="news-item">
<div class="news-date">{{ talk.date }}</div>
<div class="news-headline">
<strong>{{ talk.title }}</strong><br>
{{ talk.venue }}{% if talk.url %} <a href="{{ talk.url }}" target="_blank" rel="noopener">Talk link</a>.{% endif %}
</div>
</div>
{% endfor %}
</div>
</div>
{% endif %}
