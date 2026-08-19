---
layout: page
title: Blog
permalink: /blog/
---

{% if site.posts.size > 0 %}
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%B %-d, %Y" }}
{% endfor %}
{% else %}
No posts yet — check back soon!
{% endif %}
