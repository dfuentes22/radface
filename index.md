---
layout: default
---

<div class="col">
        {% for post in site.categories['Front'] %}
        <div class="photo">
            <a href="{{ post.url }}"><img src="../img/{{ post.image }}" alt="..."></a>
        </div>
        {% endfor %}
</div>