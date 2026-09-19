---
title: Team
description: "Current members of the CoDS Lab at Concordia University, and alumni with their placements at Mila–McGill, IBM, Verily, Waterloo, National Bank of Canada, Desjardins and Snowflake."
---
# Team

<p class="lede">The Concordia Data Systems (CoDS) Lab: one postdoctoral researcher, five PhD students and one MSc student, each attached to a thrust of the <a href="/research/">research program</a>.</p>

## Current members

<div class="table-wrap">
<table>
  <caption class="sr-only">Current lab members</caption>
  <thead><tr><th scope="col">Name</th><th scope="col">Role</th><th scope="col">Topic</th><th scope="col">Expected completion</th></tr></thead>
  <tbody>
  {%- for m in site.data.team.postdoc %}<tr><th scope="row">{{ m.name }}</th><td data-label="Role">Postdoctoral researcher</td><td data-label="Topic">{{ m.topic }}</td><td data-label="Expected completion">{{ m.until }}</td></tr>{% endfor %}
  {%- for m in site.data.team.phd %}<tr><th scope="row">{{ m.name }}</th><td data-label="Role">PhD</td><td data-label="Topic">{{ m.topic }}</td><td data-label="Expected completion">{{ m.until }}</td></tr>{% endfor %}
  {%- for m in site.data.team.msc %}<tr><th scope="row">{{ m.name }}</th><td data-label="Role">MSc</td><td data-label="Topic">{{ m.topic }}</td><td data-label="Expected completion">{{ m.until }}</td></tr>{% endfor %}
  </tbody>
</table>
</div>
<p class="small muted">Three PhD students and one MSc student joined in September 2026.</p>

## Alumni and placements

<div class="table-wrap">
<table>
  <thead><tr><th scope="col">Name</th><th scope="col">Degree</th><th scope="col">Year</th><th scope="col">Now</th></tr></thead>
  <tbody>
  {%- for a in site.data.team.alumni %}
  <tr><th scope="row">{{ a.name }}{% if a.note %}<br><span class="small muted" style="font-weight:400">{{ a.note }}</span>{% endif %}</th><td data-label="Degree">{{ a.degree }}</td><td data-label="Year">{{ a.year }}</td><td data-label="Now">{{ a.where }}</td></tr>
  {%- endfor %}
  </tbody>
</table>
</div>

## Join the lab

See [contact and recruitment](/contact/) for what the lab looks for.
