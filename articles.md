---
layout: page
title: Articles
lang: en
---

In this section you will find the information you need of all articles

## Categories
{% for category in site.categories %}
<p>
  <a href="#{{ category[0] | slugify }}">
    {{ category[0] | capitalize }}
  </a>
 ({{ category[1].size }})
</p>
{% endfor %}


## Articles
{% assign posts=site.posts | where:"lang", page.lang %}
<ul>
{% for post in posts %}

    <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        {% assign langs=site.posts | where:"ref", post.ref %}
        {% for page in langs %}
          <a href="{{ page.url }}">[{{ page.lang }}]</a>
        {% endfor %}
    </li>
{% endfor %}
</ul>
