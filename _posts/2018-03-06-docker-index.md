---
layout: post
title:  "Docker Index"
date:   2018-03-06 20:47:52 -0300
categories: index
lang: en
ref: 2018-03-06-docker-index
---
{% assign category_name = 'docker' %}
{% assign posts=site.posts | where:"lang", page.lang %}

{% for post in posts %}
{% if post.categories contains category_name %}
  <a href="{{ post.url }}">{{ post.title }} {{ post.date | date: "%Y-%m-%d"  }}</a>
{% endif %}
{% endfor %}
