---
layout: page
permalink: /categories/
title: Categories
lang: en
---

<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}

    <h3 class="category-head" id="{{ category_name }}">{{ category_name }}</h3>
    {% assign posts=site.posts | where:"lang", page.lang %}
    {% for post in posts  %}
          <article>
          {% if post.categories contains category_name %}
            <a href="{{ post.url }}">{{ post.title }}</a>
            {% assign langs=site.posts | where:"ref", post.ref %}
            {% for page in langs %}
              <a href="{{ page.url }}">{{ page.lang }}</a>
            {% endfor %}
          {% endif %}
          </article>
    {% endfor %}


{% endfor %}
