---
layout: default
title: Publications
---
<section class="page-hero compact"><div class="container narrow"><div class="eyebrow">PUBLICATIONS</div><h1>Publications</h1><p class="lead">Research outputs associated with NONLIN.</p></div></section>
<section class="section"><div class="container narrow">
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% assign current_year = '' %}
{% for pub in pubs %}{% assign year = pub.date | date: "%Y" %}{% if year != current_year %}<h2 class="year-heading">{{ year }}</h2>{% assign current_year = year %}{% endif %}
<article class="publication-item wide"><div><h3>{{ pub.title }}</h3><p>{{ pub.authors }}</p><p class="journal">{{ pub.journal }}{% if pub.volume %}, {{ pub.volume }}{% endif %}{% if pub.pages %}, {{ pub.pages }}{% endif %}</p>{% if pub.doi %}<a class="text-link small-link" href="https://doi.org/{{ pub.doi }}">https://doi.org/{{ pub.doi }} ↗</a>{% endif %}</div></article>
{% endfor %}
</div></section>
