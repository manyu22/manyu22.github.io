---
layout: default
title: About Me
description: “It is error only, and not truth, that shrinks from inquiry.“ - Thomas Paine
permalink: /about/
show_links: true
---
{% if site.owner.avatar contains 'http://' %}
<img src="{{ site.owner.avatar }}" class="bio-photo" alt="{{ site.owner.name }} bio photo">
{% elsif site.owner.avatar contains 'https://' %}
<img src="{{ site.owner.avatar }}" class="bio-photo" alt="{{ site.owner.name }} bio photo">
{% elsif site.owner.avatar %}
<img src="{{ site.url }}/images{{ site.owner.avatar }}" class="bio-photo" alt="{{ site.owner.name }} bio photo">
{% endif %}
I am Abhimanyu Panwar, a software engineer, nature lover, sports enthusiast, and an avid reader of non-fiction. I seek order in various aspects of life in general. I yearn to be wise and to simplify life, while practicing the art of not giving too much importance to oneself.