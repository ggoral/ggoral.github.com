---
layout: page
permalink: /categories/
title: Categories
---


<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <h3 class="category-head" id="{{ category_name }}">{{ category_name }}</h3>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
        <a href="{{ post.url }}">{{ post.title }} [{{ post.lang }}]</a>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>
