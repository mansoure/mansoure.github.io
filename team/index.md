---
title: Team
description: "Current members of the CoDS Lab at Concordia University, and graduated students with their current positions at Mila–McGill, Verily, the University of Waterloo, IBM, National Bank of Canada, Desjardins and Snowflake."
heading: "Team"
lede: "The Concordia Data Systems (CoDS) Lab: one postdoctoral researcher, five PhD students and one MSc student, each attached to a thrust of the research program."
---

{%- comment %} Topic strings may end in "(co-supervised with X)"; that part is shown on its own line. {% endcomment %}

## Current members

{% assign groups = "postdoc|Postdoctoral researcher,phd|PhD students,msc|Master’s student" | split: "," %}
{%- for g in groups %}
{%- assign gp = g | split: "|" %}
<h3>{{ gp[1] }}</h3>
<ul class="rows people">
{%- case gp[0] %}
{%- when "postdoc" %}{% assign members = site.data.team.postdoc %}
{%- when "phd" %}{% assign members = site.data.team.phd %}
{%- else %}{% assign members = site.data.team.msc %}
{%- endcase %}
{%- for m in members %}
  {%- assign tp = m.topic | split: " (co-supervised with " %}
  <li>
    <span class="name">{{ m.name }}</span>
    <span>{{ tp[0] }}{% if tp[1] %}<span class="d">Co-supervised with {{ tp[1] | remove: ")" }}</span>{% endif %}{% if m.work != "" %}<span class="d">Work: {{ m.work }}</span>{% endif %}</span>
    <span class="r">{{ m.until }}</span>
  </li>
{%- endfor %}
</ul>
{%- endfor %}
<p class="small sub">Three PhD students and one MSc student joined in September 2026.</p>

## Graduated PhD students

<ul class="rows alumni">
{%- for a in site.data.team.phd_alumni %}
  <li>
    <span class="name">{{ a.name }}</span>
    <span>PhD {{ a.year }}{% if a.honour %}, {{ a.honour }}{% endif %}<span class="d">At CoDS: {{ a.work }}</span></span>
    <span class="r">{{ a.where }}</span>
  </li>
{%- endfor %}
</ul>

## Master’s and undergraduate graduates

<ul class="rows alumni">
{%- for a in site.data.team.msc_alumni %}
  <li>
    <span class="name">{{ a.name }}</span>
    <span>{{ a.degree }}{% if a.year != "" %} {{ a.year }}{% endif %}{% if a.work != "" %}<span class="d">At CoDS: {{ a.work }}</span>{% endif %}</span>
    <span class="r">{{ a.where }}</span>
  </li>
{%- endfor %}
</ul>

## Join the lab

See [contact and recruitment](/contact/) for what the lab looks for.
