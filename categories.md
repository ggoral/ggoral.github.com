---
layout: page
permalink: /categories/
title: Categories
lang: en
---

<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first  }}{% endcapture %}

    <h3 class="category-head" id="{{ category_name }}">{{ category_name | capitalize }}</h3>
    {% assign posts=site.posts | sort: 'date' %}
    {% for post in posts  %}
          <article>
          {% if post.categories contains category_name %}
            <a href="{{ post.url }}">{{ post.title }}</a>
          {% endif %}
          </article>
    {% endfor %}
{% endfor %}
