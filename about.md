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
I am Abhimanyu Panwar, software engineer, nature lover, sports enthusiast, reads non-fiction and I seek order in things and life in general. I yearns to be wise and simplify life, trying the art of not giving too importance to oneself.