---
title: News
description: "News from Essam Mansour and the CoDS Lab at Concordia University: accepted papers, invited talks, student milestones, grants and conference leadership."
heading: "News"
---

<ul class="rows">
{%- for n in site.data.news %}
  <li>
    <time class="k" datetime="{{ n.date | date: '%Y-%m-%d' }}">{% if n.precision == 'year' %}{{ n.date | date: '%Y' }}{% else %}{{ n.date | date: '%B %Y' }}{% endif %}</time>
    <div><span class="t">{% if n.link %}<a href="{{ n.link }}">{{ n.title }}</a>{% else %}{{ n.title }}{% endif %}</span>
    {%- if n.body %}<p>{{ n.body }}</p>{% endif %}</div>
  </li>
{%- endfor %}
</ul>

## Earlier news (2020 to 2021)

<ul class="rows">
{%- for post in site.posts %}
  <li>
    <time class="k" datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%B %Y' }}</time>
    <div><span class="t"><a href="{{ post.url }}">{{ post.title }}</a></span></div>
  </li>
{%- endfor %}
</ul>
