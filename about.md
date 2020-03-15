---
layout: default
title: About Me
description: “It is error only, and not truth, that shrinks from inquiry.“ - Thomas Paine
permalink: /about/
show_links: true
---
# About
{% if site.owner.avatar contains 'http://' %}
<img src="{{ site.owner.avatar }}" class="bio-photo" alt="{{ site.owner.name }} bio photo">
{% elsif site.owner.avatar contains 'https://' %}
<img src="{{ site.owner.avatar }}" class="bio-photo" alt="{{ site.owner.name }} bio photo">
{% else %}
<img src="{{ site.url }}/images{{ site.owner.avatar }}" class="bio-photo" alt="{{ site.owner.name }} bio photo">
{% endif %}
My name is Abhimanyu Panwar. I am a Software Engineer by profession and a polymath by aspiration. I am a wildlife and nature enthusiast. A believer of gandhian values. Always on the lookout for simplfying things.
