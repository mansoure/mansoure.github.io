---
title: Team
description: "Current members of the CoDS Lab at Concordia University, and graduated students with their current positions at Mila–McGill, Verily, the University of Waterloo, IBM, National Bank of Canada, Desjardins and Snowflake."
---
# Team

<p class="lede">The Concordia Data Systems (CoDS) Lab: one postdoctoral researcher, five PhD students and one MSc student, each attached to a thrust of the <a href="/research/">research program</a>.</p>

## Current members

<div class="table-wrap">
<table>
  <thead><tr><th scope="col">Name</th><th scope="col">Role</th><th scope="col">Topic</th><th scope="col">Expected</th></tr></thead>
  <tbody>
  {%- assign current = site.data.team.postdoc | concat: site.data.team.phd | concat: site.data.team.msc %}
  {%- for m in current %}
  <tr>
    <th scope="row">{{ m.name }}{% if m.work != "" %}<br><span class="sub">{{ m.work }}</span>{% endif %}</th>
    <td data-label="Role">{{ m.role }}</td>
    <td data-label="Topic">{{ m.topic }}</td>
    <td data-label="Expected">{{ m.until }}</td>
  </tr>
  {%- endfor %}
  </tbody>
</table>
</div>
<p class="small muted">Three PhD students and one MSc student joined in September 2026.</p>

## Graduated PhD students

<p>Where they are now, and what they built here.</p>

<ul class="cards alumni">
{%- for a in site.data.team.phd_alumni %}
  <li class="card">
    <span class="meta">PhD {{ a.year }}{% if a.honour %} · {{ a.honour }}{% endif %}</span>
    <h3>{{ a.name }}</h3>
    {%- if a.where != "" %}<p class="now"><strong>Now:</strong> {{ a.where }}</p>{% endif %}
    <p class="who"><strong>At CoDS:</strong> {{ a.work }}</p>
  </li>
{%- endfor %}
</ul>

## Master's and undergraduate graduates

<div class="table-wrap">
<table>
  <thead><tr><th scope="col">Name</th><th scope="col">Degree</th><th scope="col">Year</th><th scope="col">Now</th><th scope="col">At CoDS</th></tr></thead>
  <tbody>
  {%- for a in site.data.team.msc_alumni %}
  <tr>
    <th scope="row">{{ a.name }}</th>
    <td data-label="Degree">{{ a.degree }}</td>
    <td data-label="Year">{{ a.year }}</td>
    <td data-label="Now">{{ a.where }}</td>
    <td data-label="At CoDS">{{ a.work }}</td>
  </tr>
  {%- endfor %}
  </tbody>
</table>
</div>

## Join the lab

See [contact and recruitment](/contact/) for what the lab looks for.
