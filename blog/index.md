---
title: Posts organized by date
---

{% for post in site.posts %}
<article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    *{{ post.date }}*
    {{ post.content }}
</article>
{% endfor %}
<!--stackedit_data:
eyJoaXN0b3J5IjpbNjUzODAyNzQ0XX0=
-->