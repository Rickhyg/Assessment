---
title: Hot-pot Gallery
layout: index
---

{% for exhibit in site.exhibits %}

<img src="{{ exhibit.image-url }}" width = 512>
<p>{{ exhibit.title }} by {{ exhibit.creator }} &nbsp;&nbsp; <a href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a></p>

{% endfor %}