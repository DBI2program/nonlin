---
layout: default
title: News
---
<section class="page-hero compact"><div class="container narrow"><div class="eyebrow">NEWS</div><h1>News from NONLIN</h1><p class="lead">Publications, meetings, milestones and other project updates.</p></div></section>
<section class="section"><div class="container news-page-grid">
{% assign newsitems = site.news | sort: 'date' | reverse %}
{% for item in newsitems %}<article class="news-card"><div class="news-thumb large"></div><div class="news-meta"><span>{{ item.category }}</span> · {{ item.date | date: "%d %B %Y" }}</div><h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2><p>{{ item.excerpt | strip_html | truncatewords: 24 }}</p><a class="text-link" href="{{ item.url | relative_url }}">Read more →</a></article>{% endfor %}
</div></section>
