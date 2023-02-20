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
    <h3>{{ page.title }}</h3>
    *{{ page.date }}*
    {{ content }}
</article>
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1OTk5MTkxMDgsMjc5NDE4NTU2XX0=
-->