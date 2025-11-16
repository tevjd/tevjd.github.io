---
layout: default
title: Tech Blog
---

# 💻 Tech Blog

Articles and tutorials on technos, security tools, and other concepts I'm learning. This is a good starting point to introduce yourself on some topics.

---

### All Posts
<ul>
  {% for post in site.categories.techno reversed %}
    <li>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html }}</p>
      <small>Posted: {{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>