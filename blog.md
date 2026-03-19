---
layout: default
title: Blog
permalink: /blog/
---

# Blog

{% if site.posts.size > 0 %}
{% for post in site.posts %}
## [{{ post.title | default: post.slug | replace: '-', ' ' | capitalize }}]({{ post.url }})

*{{ post.date | date: "%d %b %Y" }}*

{{ post.excerpt }}

---
{% endfor %}
{% else %}
No posts published yet.
{% endif %}

[Back to homepage](/)
