---
layout: default
title: کتاب‌ها
lang: fa
dir: rtl
permalink: /fa/books/
---
<section class="collection-header">
  <p class="eyebrow">کتاب‌ها</p>
  <h1>کتاب‌ها</h1>
</section>

<section class="card-grid">
{% assign items = site.books_fa | sort: "year" | reverse %}
{% for item in items %}
  <article class="card">
    <p class="meta">{{ item.year }}{% if item.publisher %} · {{ item.publisher }}{% endif %}</p>
    <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
    {% if item.excerpt %}<p class="excerpt">{{ item.excerpt }}</p>{% endif %}
  </article>
{% endfor %}
</section>
