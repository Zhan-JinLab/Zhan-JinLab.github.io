---
layout: default
title: 首页
lang: zh
---

<div class="hero-section mission-hero">
    <div class="hero-inner">
        <h1>詹/金实验室</h1>
        <p>通过创新的 CAR-T 细胞工程和转化研究，推进脑肿瘤的癌症神经科学与免疫治疗</p>
    </div>
</div>

<div class="home-section">
    <h2>我们的使命</h2>
    <p>胶质母细胞瘤（GBM）是最具毁灭性的脑肿瘤之一，当前治疗选择有限，预后差。实验室聚焦脑肿瘤与免疫系统的复杂互作，开发新型免疫治疗策略，尤其是 CAR-T 细胞疗法，以克服免疫抑制性肿瘤微环境，改善患者预后。</p>
    <p>我们融合癌症神经科学、癌症免疫学与细胞工程，研究脑肿瘤如何逃避免疫监视，并探索如何激活和引导免疫系统精确杀伤肿瘤。</p>
</div>

<div class="focus-image">
    <img src="{{ '/assets/images/ResearchFocus.jpg' | relative_url }}" alt="研究方向示意">
</div>

<div class="home-section research-focus-block single-column">
    <div class="research-text">
        <h2>研究方向</h2>
        <div class="research-grid single-row">
            <div class="research-area">
                <h3>癌症神经科学</h3>
                <p>探索脑肿瘤及其微环境的独特神经生物学特征，寻找新的治疗靶点。</p>
            </div>
            <div class="research-area">
                <h3>癌症免疫学</h3>
                <p>研究胶质母细胞瘤的免疫失调机制，制定增强抗肿瘤免疫的策略。</p>
            </div>
            <div class="research-area">
                <h3>CAR-T 细胞治疗</h3>
                <p>工程化 CAR-T 细胞，提升肿瘤靶向性、持久性及对实体瘤的疗效。</p>
            </div>
            <div class="research-area">
                <h3>胶质母细胞瘤研究</h3>
                <p>解析治疗耐药机制，开发联合治疗策略。</p>
            </div>
            <div class="research-area">
                <h3>神经肿瘤学</h3>
                <p>将实验室发现转化为临床应用，改善脑肿瘤患者的治疗结局。</p>
            </div>
            <div class="research-area">
                <h3>嵌合受体/蛋白工程</h3>
                <p>设计与优化嵌合受体和蛋白，增强免疫细胞功能、特异性与疗效持久性。</p>
            </div>
        </div>
    </div>
</div>

<div class="home-section">
    <h2>最新动态</h2>
    <ul class="news-list">
    {% for post in site.posts limit:3 %}
        <li class="news-item">
            <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
            <div class="news-date">{{ post.date | date: "%Y年%m月%d日" }}</div>
            <p class="news-excerpt">{{ post.excerpt }}</p>
        </li>
    {% endfor %}
    </ul>
    <p style="text-align: center; margin-top: 2rem;">
        <a href="{{ '/news/' | relative_url }}" style="font-weight: 500;">查看全部新闻 →</a>
    </p>
</div>

<div class="home-section">
    <h2>加入我们</h2>
    <p>欢迎对免疫治疗、神经科学、分子/细胞生物学或生物工程充满热情的学生、博士后和访问学者加入。若您期待在脑肿瘤免疫治疗与转化研究中做出突破，欢迎联系。</p>
    <p style="text-align: center; margin-top: 1.5rem;">
        <a href="{{ '/contact/' | relative_url }}" style="font-weight: 500; font-size: 1.1rem;">联系我们 →</a>
    </p>
</div>

