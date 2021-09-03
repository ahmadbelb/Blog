---
layout: archive
title: "Letters"
permalink: /letters/
author_profile: true
---
<link rel="apple-touch-icon" sizes="180x180" href="https://ahmadbelb.github.io/Blog/images/favicon/apple-touch-icon.png">
{% include image.html url="https://ahmadbelb.github.io/Blog/images/writing.jpg"%}

These are the letters I send out annually to help stay connected with my community. 

{% include base_path %}

{% for post in site.letters reversed %}
  {% include archive-single.html %}
{% endfor %}
