---
layout: default
title: Categories
description: “When one has been threatened with a great injustice, one accepts a smaller as a favour.“ - Jane Welsh Carlyle
permalink: /categories/
show_links: true
---
All the posts listed by their categories.

{% for category in site.categories %}
### {{ category[0] }}
---
{% for post in category[1] %}
  :{{post.emoticon}}: {{ post.date | date_to_string }} [{{ post.title }}]({{ post.url }})
{% endfor %}
{% endfor %}