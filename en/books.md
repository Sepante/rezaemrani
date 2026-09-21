---
layout: default
title: Books
lang: en
dir: ltr
permalink: /en/books/
---
<section class="collection-header">
  <p class="eyebrow">Books</p>
  <h1>Books</h1>
</section>

<section class="card-grid">
{% assign items = site.books_en | sort: "year" | reverse %}
{% for item in items %}
  <article class="card">
    <p class="meta">{{ item.year }}{% if item.publisher %} · {{ item.publisher }}{% endif %}</p>
    <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
    {% if item.excerpt %}<p class="excerpt">{{ item.excerpt }}</p>{% endif %}
  </article>
{% endfor %}
</section>
