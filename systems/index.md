---
title: Systems and Benchmarks
description: "Open-source systems and benchmarks from the CoDS Lab: MAFBench, MemState, Chatty-KG, ReSequel, OCR-APT, RAGvis, CatDB, Chatty-Gen, and the foundational KGLiDS, KGNet, KGQAn and KGpip."
---
# Systems and benchmarks

<p class="lede">The CoDS-GCS GitHub organization open-sources more than 30 repositories. Each ships with reproducible benchmarks, documentation and an associated peer-reviewed publication.</p>

<p class="callout"><strong>External adoption.</strong> KGLiDS was adopted by Google and Kaggle teams for production data science workflows. Its follow-on system, RAGvis, is released inside Google's own GitHub organization (<a href="https://github.com/google/ragvis">google/ragvis</a>) and was published at EMNLP 2025.</p>

## Agentic AI systems and benchmarks (2025 to 2027)

<ul class="cards">
{%- for s in site.data.systems %}{% if s.group == 'agentic' %}
  <li class="card" id="{{ s.id }}">
    <span class="meta">{{ s.venue }}</span>
    <h3>{{ s.name }}</h3>
    <p>{{ s.desc }}</p>
    {%- if s.note %}<p class="who"><strong>{{ s.note }}</strong></p>{% endif %}
    <div class="links"><a href="{{ s.code }}">Code</a><a href="{{ s.paper }}">Paper</a></div>
  </li>
{%- endif %}{% endfor %}
</ul>

<h2 id="foundational">Foundational systems</h2>

<ul class="cards">
{%- for s in site.data.systems %}{% if s.group == 'foundational' %}
  <li class="card" id="{{ s.id }}">
    <span class="meta">{{ s.venue }}</span>
    <h3>{{ s.name }}</h3>
    <p>{{ s.desc }}</p>
    {%- if s.note %}<p class="who"><strong>{{ s.note }}</strong></p>{% endif %}
    <div class="links"><a href="{{ s.code }}">Code</a><a href="{{ s.paper }}">Paper</a></div>
  </li>
{%- endif %}{% endfor %}
</ul>

I also contribute to [aurum-datadiscovery](https://github.com/mitdbg/aurum-datadiscovery) (MIT DBG), and to E-Store (VLDB 2015) and Solid (WWW 2016, with Tim Berners-Lee).

## Earlier research projects

These projects from before the current program keep their original pages:

- [The Data Civilizer System](/research/dc/): end-to-end data discovery, integration and cleaning in large enterprises.
- [Managing Linked Data at Scale (Lusail)](/research/lusail/): querying, integrating and sharing geo-distributed RDF graphs.
- [Elastic in-memory OLTP (E-Store)](/research/estore/)
- [Large-scale analytics on strings](/research/starDB/)
