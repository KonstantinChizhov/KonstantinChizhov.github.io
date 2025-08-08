---
layout: default
title: Главная
---
# Записки разработчика

## Последние статьи:

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
*Published: {{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt | strip_html | truncatewords: 30 }}
{% endfor %}