---
layout: default
home: true
title: "Essam Mansour: agents that operate safely on organizational data"
description: "Essam Mansour, Tenured Associate Professor at Concordia University and Head of the CoDS Lab. General Chair of IEEE ICDE 2026. Builds AI agents that operate safely on organizational data, grounding their architecture in data systems and knowledge graphs to automate enterprise operations."
---

<ul class="recently" aria-label="Recently">
  <li class="label">Recently</li>
{%- assign home_news = site.data.news | where_exp: "n", "n.home != false" %}
{%- for n in home_news limit:3 %}
  <li><a href="{{ n.link | default: '/news/' }}">{{ n.title }}</a></li>
{%- endfor %}
</ul>

<h2>What we work on</h2>
<p>Agents have no governed way to accumulate what an organization knows, and no way to establish that what they accumulated is trustworthy. We work on this at the data layer, and release our systems open source through <a href="https://github.com/CoDS-GCS">CoDS-GCS</a>.</p>
<ul class="rows plain">
{%- for t in site.data.thrusts %}
  <li><a class="name" href="/research/#{{ t.id }}">{{ t.title }}</a><span class="d">{{ t.short }}</span></li>
{%- endfor %}
</ul>
<p class="more"><a href="/research/">The research program</a></p>

<h2>Recent systems</h2>
<ul class="rows">
{%- for s in site.data.systems %}{% if s.featured %}
  <li><span class="k">{{ s.venue | remove: " (main)" }}</span><span><a class="name" href="/systems/#{{ s.id }}">{{ s.name }}</a>, {{ s.short | default: s.desc }}</span></li>
{%- endif %}{% endfor %}
</ul>
<p class="sub">KGLiDS was adopted by Google and Kaggle teams, and RAGvis is released in Google’s own GitHub organization.</p>
<p class="more"><a href="/systems/">All systems and benchmarks</a></p>

<h2>News</h2>
<ul class="rows">
{%- for n in home_news offset:3 limit:4 %}
  <li><time class="k" datetime="{{ n.date | date: '%Y-%m-%d' }}">{% if n.precision == 'year' %}{{ n.date | date: '%Y' }}{% else %}{{ n.date | date: '%B %Y' }}{% endif %}</time><span>{% if n.link %}<a href="{{ n.link }}">{{ n.title }}</a>{% else %}{{ n.title }}{% endif %}</span></li>
{%- endfor %}
</ul>
<p class="more"><a href="/news/">News archive</a></p>
