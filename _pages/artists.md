---
layout: default
permalink: /artists/
title: 'artists:all'
description: 'artists:all'
og-image: ''
---

# {{ page.title }}

{% include menu-artists.html %}

<section>
  {% for file in site.static_files %}
    {% if file.path contains 'assets/img/artists/' %}
      {% include article.html %}
    {% endif %}
  {% endfor %}
</section>
