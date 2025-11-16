---
layout: default
title: Projects
---

# 🛠️ My Projects

A showcase of the tools and scripts I'm building.

---

### All Posts
<ul>
  {% for post in site.categories.project reversed %}
    <li>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html }}</p>
      <small>Posted: {{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>