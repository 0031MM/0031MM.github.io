---
# Feel free to add content and custom Front Matter to this file.
layout: default
title: Home
---
{% for post in site.posts limit:5 %}
[{{ post.title }}]({{ post.url }})
{% endfor %}
