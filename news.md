---
layout: page
title: News
subtitle: Latest updates from the Zhan/Jin Laboratory
---

<div class="news-list">
{% for post in site.posts %}
    <li class="news-item">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <div class="news-date">{{ post.date | date: "%B %d, %Y" }}</div>
        <p class="news-excerpt">{{ post.excerpt }}</p>
        <a href="{{ post.url | relative_url }}">Read more →</a>
    </li>
{% endfor %}
</div>

{% if site.posts.size == 0 %}
<div class="coming-soon">
    <p>News updates will be posted here. Stay tuned for the latest developments from our laboratory.</p>
</div>
{% endif %}

