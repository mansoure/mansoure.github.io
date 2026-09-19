---
layout: default
home: true
title: "Essam Mansour: agents that operate safely on organizational data"
description: "Essam Mansour, Tenured Associate Professor at Concordia University and Head of the CoDS Lab. General Chair of IEEE ICDE 2026. Research on governed agent memory, action contracts, validation of agent-generated code and agent security."
---
<div class="hero-band">
<section class="hero wrap">
  <div class="hero-text">
    <p class="eyebrow">Tenured Associate Professor · Concordia University</p>
    <h1>Essam Mansour</h1>
    <p class="role">Head, Concordia Data Systems (CoDS) Lab · Montreal</p>
    <p class="position">Essam Mansour builds agents that operate safely on organizational data. Architecture, not only model capability, decides whether an enterprise agent works.</p>
    <ul class="status" aria-label="Current roles">
      <li><strong>General Chair</strong>, IEEE ICDE 2026</li>
      <li><strong>Editor</strong>, ACM SIGMOD Blog</li>
      <li><strong>Head</strong> of the CoDS Lab</li>
    </ul>
    <ul class="actions">
      <li><a class="btn" href="/cv/mansour-cv.pdf">CV (PDF)</a></li>
      <li><a href="https://scholar.google.com/citations?user=dqgckDgAAAAJ">Google Scholar</a></li>
      <li><a href="https://dblp.org/pid/m/EssamMansour.html">DBLP</a></li>
      <li><a href="https://github.com/CoDS-GCS">GitHub</a></li>
      <li><a href="https://www.linkedin.com/in/emansour">LinkedIn</a></li>
      <li><a rel="me" href="https://discuss.systems/@emansour">Mastodon</a></li>
    </ul>
  </div>
  <img class="hero-photo" src="/images/essam-2024-light.jpg" width="720" height="851" alt="Portrait of Essam Mansour" fetchpriority="high">
</section>
</div>

<div class="wrap">
<section class="recent" aria-labelledby="recent-h">
  <h2 id="recent-h">Recent</h2>
  <ol>
  {%- for n in site.data.news limit:4 %}
    <li>
      <time datetime="{{ n.date | date: '%Y-%m-%d' }}">{% if n.precision == 'year' %}{{ n.date | date: '%Y' }}{% else %}{{ n.date | date: '%B %Y' }}{% endif %}</time>
      <a href="{{ n.link | default: '/news/' }}">{{ n.title }}</a>
    </li>
  {%- endfor %}
  </ol>
</section>

<h2>What we work on</h2>
<p class="lede">The barrier to enterprise agents is not model capability. It is that agents have no governed way to accumulate what an organization knows, and no way to establish that what they accumulated is trustworthy. We attack it at the data layer.</p>
<ul class="cards">
{%- for t in site.data.thrusts %}
  <li class="card">
    <h3><a href="/research/#{{ t.id }}">{{ t.title }}</a></h3>
    <p>{{ t.short }}</p>
  </li>
{%- endfor %}
</ul>
<p class="section-more"><a href="/research/">The research program →</a></p>

<h2>Recent systems</h2>
<p class="lede">Open-source systems and benchmarks from the CoDS-GCS organization, published at SIGMOD, VLDB, EMNLP, ICDE and CCS.</p>
<ul class="cards">
{%- for s in site.data.systems %}{% if s.featured %}
  <li class="card">
    <span class="meta">{{ s.venue }}</span>
    <h3><a href="/systems/#{{ s.id }}">{{ s.name }}</a></h3>
    <p>{{ s.desc }}</p>
  </li>
{%- endif %}{% endfor %}
</ul>
<p class="callout"><strong>External adoption.</strong> KGLiDS was adopted by Google and Kaggle teams, and its follow-on system RAGvis is released in Google's own GitHub organization.</p>
<p class="section-more"><a href="/systems/">All systems and benchmarks →</a></p>

<h2>Latest news</h2>
<ul class="news">
{%- for n in site.data.news limit:6 %}
  <li>
    <time datetime="{{ n.date | date: '%Y-%m-%d' }}">{% if n.precision == 'year' %}{{ n.date | date: '%Y' }}{% else %}{{ n.date | date: '%B %Y' }}{% endif %}</time>
    <div><span class="t">{% if n.link %}<a href="{{ n.link }}">{{ n.title }}</a>{% else %}{{ n.title }}{% endif %}</span>
    {%- if n.body %}<p>{{ n.body }}</p>{% endif %}</div>
  </li>
{%- endfor %}
</ul>
<p class="section-more"><a href="/news/">News archive →</a></p>

</div>
