---
layout: page
title: Articles
lang: en
---

This is a few list of all articles

{% assign posts=site.posts %}
<ul>
{% for post in posts %}
    <li>
        <a href="{{ post.url }}">{{ post.title }} [{{ post.lang }}]</a>
    </li>
{% endfor %}

</ul>

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
