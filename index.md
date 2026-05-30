---
# Feel free to add content and custom Front Matter to this file.
layout: default
title: 31MM
---

<div id="projects-list">
{% for post in site.posts limit:100 %}
<div>
  <a href="{{ post.url | relative_url }}" class="project-card">
    {% if post.image %}
    <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
    {% else %}
    <div class="project-card__placeholder"></div>
    {% endif %}
    <span class="project-card__title">{{ post.title }}</span>
  </a>
</div>
{% endfor %}
</div>