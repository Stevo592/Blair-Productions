---
layout: default
title: tech
---

# tech

<ul>
  {% for page in site.pages %}
    {% if page.path contains "tech/" and page.path != "tech/index.md" %}
      <li>
        <a href="{{ page.url }}">{{ page.title }}</a> - {{ page.date | date: "%B %d, %Y" }}
      </li>
    {% endif %}
  {% endfor %}
</ul>