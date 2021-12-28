---
title: Common Ingredients
layout: index
---

<p> 
    Come with us to learn about the common ingredients of hotpot! 
</p>

{% for ingredient in site.ingredients %}

<a href = "/{{ingredient.title}}"><img src="{{ ingredient.image-url }}" width = 512></a>
<h4>{{ ingredient.title }}</h4>
<p>Created by {{ ingredient.creator }} &nbsp;&nbsp; <a href="{{ exhibit.licence-url }}">{{ ingredient.licence }}</a></p>

{% endfor %}
