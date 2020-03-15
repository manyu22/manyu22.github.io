---
layout: default
title: The Sage
description: “In a consumer society there are inevitably two kinds of slaves, the prisoners of addiction and the prisoners of envy.” — Ivan Illich
show_links: true
---
## Latest Posts

{% for post in site.posts %}
---
:{{post.emoticon}}: {{ post.date | date_to_string }} [{{ post.title }}]({{ post.url }})
##### tags: {% for tag in post.tags %} `{{tag}}` {% endfor %}
{% endfor %}
