---
title: Systems and Benchmarks
description: "Open-source systems and benchmarks from the CoDS Lab: MAFBench, MemState, Chatty-KG, ReSequel, OCR-APT, RAGvis, CatDB, Chatty-Gen, and the foundational KGLiDS, KGNet, KGQAn and KGpip."
heading: "Systems and benchmarks"
lede: "The CoDS-GCS GitHub organization open-sources more than 30 repositories, each with reproducible benchmarks, documentation and a peer-reviewed paper."
---


<p>KGLiDS was adopted by Google and Kaggle teams for production data science workflows. Its follow-on system, RAGvis, is released inside Google’s own GitHub organization (<a href="https://github.com/google/ragvis">google/ragvis</a>) and was published at EMNLP 2025.</p>

## Agentic AI systems and benchmarks (2025 to 2027)

<ul class="rows three">
{%- for s in site.data.systems %}{% if s.group == 'agentic' %}
  <li id="{{ s.id }}">
    <span class="k">{{ s.venue }}</span>
    <span><span class="name">{{ s.name }}</span>. {{ s.desc }}{% if s.note %}<span class="d">{{ s.note }}</span>{% endif %}</span>
    <span class="r links"><a href="{{ s.paper }}">Paper</a><a href="{{ s.code }}">Code</a></span>
  </li>
{%- endif %}{% endfor %}
</ul>

<h2 id="foundational">Foundational systems</h2>

<ul class="rows three">
{%- for s in site.data.systems %}{% if s.group == 'foundational' %}
  <li id="{{ s.id }}">
    <span class="k">{{ s.venue }}</span>
    <span><span class="name">{{ s.name }}</span>. {{ s.desc }}{% if s.note %}<span class="d">{{ s.note }}</span>{% endif %}</span>
    <span class="r links"><a href="{{ s.paper }}">Paper</a><a href="{{ s.code }}">Code</a></span>
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
