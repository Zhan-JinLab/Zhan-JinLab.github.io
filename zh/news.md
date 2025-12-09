---
layout: page
title: 新闻
subtitle: 实验室最新动态
lang: zh
---

<div class="news-list">
{% for post in site.posts %}
    <li class="news-item">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <div class="news-date">{{ post.date | date: "%Y年%m月%d日" }}</div>
        <p class="news-excerpt">{{ post.excerpt }}</p>
        <a href="{{ post.url | relative_url }}">阅读全文 →</a>
    </li>
{% endfor %}
</div>

{% if site.posts.size == 0 %}
<div class="coming-soon">
    <p>新闻更新即将发布，敬请期待。</p>
</div>
{% endif %}

