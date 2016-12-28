---
layout: default
title: Table of Contents
page_class: bk-toc
---

{% for categ in site.categories %}
## {{ categ[0] }}
<ul>
  {% for post in categ[1] reversed %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
{% endfor %}

