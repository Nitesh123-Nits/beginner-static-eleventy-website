---
title: My first page
layout: base.njk
---
 Hello JamStack!
<ul class="ul-list">
{% for post in collections.posts | reverse %}

- [{{ post.data.title  }}]({{ post.url }})

{% endfor %}
</ul>