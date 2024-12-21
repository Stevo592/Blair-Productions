---
layout: default
title: Recipes
---

# Recipes

<ul>
  {% for recipe in site.pages %}
    {% if recipe.path contains "recipes/" and recipe.path != "recipes/index.md" %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a> - {{ recipe.date | date: "%B %d, %Y" }}
      </li>
    {% endif %}
  {% endfor %}
</ul>