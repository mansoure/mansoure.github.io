---
title: Publications
description: "Selected publications by Essam Mansour, grouped by theme: agentic AI, memory and safety; LLM and knowledge graph systems; data systems foundations. Papers at SIGMOD, VLDB, ICDE, EMNLP, EACL and CCS."
---
# Publications

<p class="lede">More than 50 papers in top-tier venues. The complete list is on <a href="https://dblp.org/pid/m/EssamMansour.html">DBLP</a> and <a href="https://scholar.google.com/citations?user=dqgckDgAAAAJ&view_op=list_works&sortby=pubdate">Google Scholar</a>. Students supervised by or working closely with me are marked with an asterisk (*).</p>

<p class="small muted">Jump to:
{%- for g in site.data.publications %} <a href="#{{ g.slug }}">{{ g.group }}</a>{% unless forloop.last %} ·{% endunless %}{% endfor %} · <a href="/publications/archive/">Earlier publications (2005–2018)</a></p>

{% for g in site.data.publications %}
<h2 id="{{ g.slug }}">{{ g.group }}</h2>
<ol class="pubs">
  {%- for p in g.items %}
  <li>
    <span class="id">{{ p.id }}</span>
    <div>
      <span class="title">{{ p.title }}</span>
      {{ p.authors | replace: 'Essam Mansour', '<strong>Essam Mansour</strong>' }}.
      <span class="venue">{{ p.venue }}, {{ p.year }}.</span>
      {%- if p.links.size > 0 %}<span class="links">{% for l in p.links %}<a href="{{ l.u }}">{{ l.l }}</a>{% endfor %}</span>{% endif %}
    </div>
  </li>
  {%- endfor %}
</ol>
{% endfor %}

## Earlier work

Papers from 2005 to 2018 on elastic OLTP, federated linked data, parallel sequence analytics and mobile data management, with PDFs, are kept in the [archive](/publications/archive/).
