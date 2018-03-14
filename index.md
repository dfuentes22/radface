---
layout: default
---

<div class="col">
        {% for post in site.categories['Front'] %}
        <div class="photo">
            <a href="{{ post.url }}"><img src="{{ site.baseurl }}/img/{{ post.image }}" alt="..."></a>
        </div>
        {% endfor %}
</div>