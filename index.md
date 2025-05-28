---
layout: home
title: Экзаменационные билеты
---

# Экзаменационные билеты по математике

Здесь собраны расписанные билеты к экзамену с математическими формулами.

## Список билетов

{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
  {% if page.title contains 'Билет' %}
  * [{{ page.title }}]({{ page.url | relative_url }})
  {% endif %}
{% endfor %}
