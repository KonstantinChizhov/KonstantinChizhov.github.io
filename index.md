---
layout: default
title: Главная
---

# Записки разработчика

## Последние статьи:
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) – {{ post.date | date: "%d.%m.%Y" }}
{% endfor %}