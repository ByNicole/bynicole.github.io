---
layout: default
---

<article class="post">
    <aside class="article-tags-header">
        <time datetime="{{ page.date }}" itemprop="datePublished">{{ page.date | date: "%e %b %Y" }}</time>
        <div>
            Tags:
            {% for tag in page.tags %}
                <a href="/blog/tags.html#{{ tag | replace: ' ', '-' }}">{{ tag }}</a>{% if forloop.last %}{% else %},{% endif %}
            {% endfor %}
        </div>
    </aside>
    <h1>{{ page.title }}</h1>
    *{{ page.date }}*
    {{ content }}
</article>
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjc5NDE4NTU2LC0xNTk5OTE5MTA4LDI3OT
QxODU1Nl19
-->