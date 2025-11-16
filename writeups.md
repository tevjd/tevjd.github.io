---
layout: default
title: Write-ups
---

# ✍️ My Write-ups

This is a complete list of my solutions and walk-throughs for CTF challenges and other security rooms.

---

### All Posts
<ul>
  {% for post in site.categories.writeup reversed %}
    <li>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html }}</p>
      <small>Posted: {{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>