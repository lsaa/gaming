---
layout: default
permalink: /post/:title
---

{{ page.date | date: "%-d %B %Y" }}

<div style="text-align:left; margin-bottom: -18px;">
    <h1 style="display: inline-block;">{{ page.title }}</h1>
    <span style="float:right; position: relative; bottom: -10px;">
        by {{ page.author }}
    </span>
</div>
<hr>
{{content}}

{% if page.tags %}
  <small>tags: <em>{{ page.tags | join: "</em> - <em>" }}</em></small>
{% endif %}
