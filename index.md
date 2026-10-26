---
layout: default
title: fun.colbywonn.com
hero: true
---

<div class="hero">
  <h1 class="crt">fun.colbywonn.com<span class="cursor" aria-hidden="true">_</span></h1>
  <p class="tagline">Toys, lists, and side projects.</p>
</div>

<div class="cards">
{%- for p in site.data.pages %}
  {%- if p.soon %}
  <div class="card soon">
    <h3>{{ p.title }}</h3>
    <p>{{ p.blurb }}</p>
    <span class="tag">Coming soon</span>
  </div>
  {%- else %}
  <a class="card" href="{{ p.url | relative_url }}">
    <h3>{{ p.title }}</h3>
    <p>{{ p.blurb }}</p>
  </a>
  {%- endif %}
{%- endfor %}
</div>
