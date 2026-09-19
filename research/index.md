---
title: Research
description: "The CoDS research program on enterprise-aware agents: governed agent memory, action contracts, validation of agent-generated code, agent security and graph foundation models. Funded by NSERC Discovery and CREATE."
---
# Research

<p class="lede">Enterprise-aware agents: moving agents from individual intelligence to organizational intelligence.</p>

The barrier to enterprise agentic deployment is not model capability. Our SIGMOD 2027 study established this empirically across nine production agent frameworks at fixed LLM and task: orchestration alone changes latency by over 60×, schema-constrained planning costs up to 32 accuracy points through parsing failures rather than reasoning failures, and communication topology swings coordination success from above 90% to below 30%. Not one framework supports controlled knowledge revision. **Architecture, not only model capability, governs agent performance.** That is a data and systems problem, and we attack it at the data layer across five coupled thrusts.

The program is funded through 2030 by NSERC Discovery and NSERC CREATE and released open source through the [CoDS-GCS](https://github.com/CoDS-GCS) organization. Every system replaces LLM self-judgment with checks against the actual data. See the [systems and benchmarks](/systems/) and the [people](/team/) behind each thrust.

{% for t in site.data.thrusts %}
<section class="thrust" id="{{ t.id }}">
  <span class="num">THRUST {{ forloop.index }}</span>
  <h2>{{ t.title }}</h2>
  <p>{{ t.text }}</p>
  <p class="people"><strong>Team:</strong>
  {%- for p in t.people %} {{ p.name }} ({{ p.role }}){% unless forloop.last %};{% endunless %}{% endfor %}</p>
  {%- if t.systems != "" %}<p class="people"><strong>Related systems:</strong> {{ t.systems }}</p>{% endif %}
</section>
{% endfor %}

## Industry and research collaborations

<ul>
<li><strong>IBM Research (2020 to present).</strong> Multi-agent AI systems for conversational question answering and enterprise data science assistance, with Ibrahim Abdelaziz and Kavitha Srinivas. Earlier work yielded KGpip.</li>
<li><strong>Google (2024 to 2025).</strong> RAG-based systems using knowledge graphs and Gemini to automate exploratory data analysis. Outcome: RAGvis (EMNLP 2025), released in Google's GitHub organization.</li>
<li><strong>National Research Council Canada (2025 to 2028).</strong> Secure knowledge sharing and agentic threat detection for the digitized construction industry.</li>
<li><strong>National Bank of Canada (2023 to 2024)</strong> and <strong>RBC Borealis AI (2022 to 2023).</strong> LLM-based risk assessment, and a linked data science platform for feature discovery and automated data preparation.</li>
<li><strong>MIT CSAIL (2013 to 2018).</strong> Technical lead on three joint projects with QCRI: E-Store, Data Civilizer and Solid.</li>
</ul>

## Earlier research

The foundations of the current program, from federated linked data to knowledge graph platforms for data science, are collected under [foundational work](/systems/#foundational).
