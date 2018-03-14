---
layout: default
title: Gallery
permalink: /gallery/
---

<div class="col">
        {% for post in site.categories['Gallery'] %}
        <div class="photo">
            <a href="{{ site.baseurl }}{{ post.url }}"><img src="../img/{{ post.image }}" alt="..."></a>
        </div>
        {% endfor %}
</div>