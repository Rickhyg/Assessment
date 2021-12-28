---
title: Meats and Protein
layout: index
---
<div style="display:grid; grid-gap:20px; margin: auto; grid-template-columns: repeat(4, 350px)">
    {% for pic in site.data.meats %}
        <div style="align-self: baseline; display: block;">
            <img src="{{ pic.image-url }}" style="width:350px; object-fit: cover;">
            <p style="display: block; margin-block-start: 1em; margin-block-end: 1em; margin-inline-start: 0px; margin-inline-end: 0px;">
                {{ pic.description }} 
                <br>picture by {{ pic.image-author }}
            </p>
            <p>
                <a href="{{ pic.license-url }}">{{ pic.license-name }}</a>
            </p>
        </div>
    {% endfor %}
</div>