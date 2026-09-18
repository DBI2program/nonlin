---
layout: default
title: Collaborators
---
<section class="page-hero compact"><div class="container narrow"><div class="eyebrow">COLLABORATORS</div><h1>Collaborators</h1><p class="lead">Researchers and partners contributing complementary expertise to NONLIN.</p></div></section>
<section class="section"><div class="container narrow collaborator-list">
{% for person in site.collaborators %}<article><h2>{{ person.name }}</h2><p class="role">{{ person.affiliation }}</p><p>{{ person.summary }}</p></article>{% endfor %}
</div></section>
