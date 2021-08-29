---
layout: archive
title: "Letters"
permalink: /letters/
author_profile: true
---

{% include image.html url="https://ahmadbelb.github.io/belbeisiahmad.github.io/images/writing.jpg"%}

These are the letters I send out annually to help stay connected with my community. 

{% include base_path %}

{% for post in site.letters reversed %}
  {% include archive-single.html %}
{% endfor %}
