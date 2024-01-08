---
layout: page
title: Artículos
---

{% for post in site.posts %}

  * <strong>{{ post.date | date_to_string }}</strong> &raquo; [ {{ post.title }} ]({{ post.url }}) <br> <i>{{ post.content | strip_html | truncate: 150 }}</i>{
{% endfor %}

