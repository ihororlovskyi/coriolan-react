---
layout: default
permalink: /
title: 'Content of Sentimony Records'
description: 'Content of Sentimony Records'
og-image: ''
---

# {{ page.title }}

<section>
  {% for file in site.static_files %}
    {% if file.path contains 'assets/img/' %}
      {% include article.html %}
    {% endif %}
  {% endfor %}
</section>
