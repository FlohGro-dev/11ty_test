---
layout: layouts/base
title: archive
permalink: /archive/
eleventyNavigation: 
    key: archive
    order: 4
---

{% include "std-icons.md" %}

## archive of all posts

{% for post in collections.posts %}
  - [{{ post.data.title }}]({{ baseUrl }}{{ post.url }}) - {{ post.data.date | isoDate }}
{% endfor %}
