---
layout: default
title: نوشته‌ها و مقالات
lang: fa
dir: rtl
permalink: /fa/publications/
---
<section class="collection-header">
  <p class="eyebrow">آثار منتخب</p>
  <h1>نوشته‌ها و مقالات</h1>
</section>

<section class="card-grid">
{% assign items = site.publications_fa | sort: "year" | reverse %}
{% for item in items %}
  <article class="card">
    <p class="meta">{{ item.year }}{% if item.venue %} · {{ item.venue }}{% endif %}</p>
    <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
    {% if item.excerpt %}<p class="excerpt">{{ item.excerpt }}</p>{% endif %}
  </article>
{% endfor %}
</section>
