---
layout: single
title: "Публікації"
permalink: /publications/
---

На цій сторінці зібрано дослідження, аналітичні матеріали, технічні огляди, нотатки та фотографії, опубліковані в межах проєкту «Приціл».

---

## Опубліковані матеріали

{% assign publications = site.posts | sort: "date" | reverse %}

{% if publications.size > 0 %}

{% for post in publications %}

### [{{ post.title }}]({{ post.url | relative_url }})

{% if post.description %}
{{ post.description }}
{% elsif post.excerpt %}
{{ post.excerpt | strip_html | truncatewords: 35 }}
{% endif %}

*Опубліковано: {{ post.date | date: "%d.%m.%Y" }}*

---

{% endfor %}

{% else %}

Поки що опублікованих матеріалів немає.

{% endif %}

## Готуються до публікації

### БМ-1Б «Грім»

Історія розробки, конструкція, озброєння, технічні особливості та аналіз можливих варіантів виконання українського бойового модуля.

*Матеріал готується до публікації.*
