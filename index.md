---
layout: default
title: Home
---
## Projects

{% for p in site.data.projects %}
### [{{ p.title }}]({{ p.url }})
{{ p.description }}
{% endfor %}

## Thoughts & ideas
{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %Y" }}
{% endfor %}
