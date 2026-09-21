---
layout: default
title: Publications
lang: en
dir: ltr
permalink: /en/publications/
---
<section class="collection-header">
  <p class="eyebrow">Selected writing</p>
  <h1>Publications</h1>
</section>

<section class="card-grid">
{% assign items = site.publications_en | sort: "year" | reverse %}
{% for item in items %}
  <article class="card">
    <p class="meta">{{ item.year }}{% if item.venue %} · {{ item.venue }}{% endif %}</p>
    <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
    {% if item.excerpt %}<p class="excerpt">{{ item.excerpt }}</p>{% endif %}
  </article>
{% endfor %}
</section>
