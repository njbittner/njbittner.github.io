---
layout: blog
title: Nathan Bittner's Personal Blog
---

{% for post in site.posts %}
{% if post.external %}
[{{post.title}} {% octicon link-external %}]({{post.external}})
{% else %}
[{{post.title}}]({{post.url}})
{% endif %} ({{post.date | date: '%B %Y' }})
{% endfor %}
