---
layout: archive
title: Projects
permalink: /projects/
author_profile: true
collection: projects
entries_layout: grid
classes: wide
image: "https://ahmadbelb.github.io/Blog/images/coverpicture.jpeg"
---
<link rel="apple-touch-icon" sizes="180x180" href="https://ahmadbelb.github.io/Blog/images/favicon/apple-touch-icon.png">
{% for post in site.projects reversed %}
  {% include archive-single.html type="grid" %}
{% endfor %}
