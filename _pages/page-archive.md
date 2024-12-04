---
layout: archive
title: "归档"
permalink: /page-archive/
author_profile: true
---

{% assign posts = site.pages | where_exp: "post", "post.hidden != true" %}
{% for post in posts %}
  {% include archive-single.html %}
{% endfor %}