---
# Feel free to add content and custom Front Matter to this file.
layout: default
title: 
permalink: /projects/
---

# What I do

Here you’ll find a selection of works that showcase my multidisciplinary approach.

{% for post in site.posts limit:20 %}
[{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%Y" }}
{% endfor %}
