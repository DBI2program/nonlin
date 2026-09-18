---
layout: default
title: Team
---
<section class="page-hero compact"><div class="container narrow"><div class="eyebrow">TEAM</div><h1>The NONLIN team</h1><p class="lead">A small research team at Radboud University studying large-scale neural interactions and cognition.</p></div></section>
<section class="section"><div class="container team-page-grid">
{% assign members = site.people | sort: 'order' %}
{% for person in members %}<article class="person-card full"><div class="portrait-placeholder">{{ person.initials }}</div><div><h2>{{ person.name }}</h2><div class="role">{{ person.role }}</div><p>{{ person.summary }}</p>{% if person.profile %}<a class="text-link" href="{{ person.profile }}">Profile ↗</a>{% endif %}</div></article>{% endfor %}
</div></section>
