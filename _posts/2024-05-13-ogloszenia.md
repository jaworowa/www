---
layout: post
title:  "Ogłoszenia i aktualności"
author: norbert
image: assets/images/4.jpg
featured: true
---
Pełna lista ogłoszeń naszej wspólnoty - zarówno aktualnych jak i historycznych.

<ul>
    {% assign posts = site.posts %}
    {% for post in posts %}
    {% if post.featured == false %}
    <li>
        <h2 class="card-title h4 serif-font"><a href="{{ post.url | absolute_url }}"> {{ post.title }} ({{ post.date | date: "%Y/%m/%d" }})</a></h2>
    </li>
    {% endif %}
    {% endfor %}
</ul>
