---
title: Basic
layout: index
---

<div style="display:flex; grid-gap:10px; margin: auto;">
    {% for pic in site.data.basic %}
        <div style="align-self: baseline;">
            <a href="{{ site.baseurl }}/Basic/{{ pic.name }}">
                <img src="{{ pic.image-url }}" style="width:350px; object-fit: cover;">
            </a>
            <p style="display: block; margin-block-start: 1em; margin-block-end: 1em; margin-inline-start: 0px; margin-inline-end: 0px;">
                <a href="{{ site.baseurl }}/Basic/{{ pic.name }}">{{ pic.name }}</a> by <a href="{{ pic.image-author-page }}">{{ pic.image-author }}</a>
            </p>
            <p>
                <a href="{{ pic.license-url }}">{{ pic.license-name }}</a>
            </p>
        </div>
    {% endfor %}
</div>