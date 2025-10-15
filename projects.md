---
# Feel free to add content and custom Front Matter to this file.
layout: default
title: Projects
permalink: /projects/
---
{% for post in site.posts limit:20 %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %Y" }}
{% endfor %}
