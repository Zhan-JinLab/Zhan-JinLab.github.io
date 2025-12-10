---
layout: page
title: 论文成果
subtitle: 在癌症免疫治疗与神经肿瘤学领域的研究贡献
lang: zh
---

我们的团队在脑肿瘤免疫生物学与新型治疗方面发表了大量论文。以下按主要负责人分组列出（论文标题沿用英文原文，便于检索）。

---

## 重点论文（部分）

### CAR-T 及免疫治疗
- CXCR1/2 修饰 CAR-T 共用 IL-8 提升实体瘤疗效（Nat Commun, 2019）
- CD70 作为胶质瘤 CAR-T 靶点（Neuro-Oncology, 2018）

### 胶质母细胞瘤生物学与耐药
- GBM 治疗现状与耐药机制综述（Pharmacol Res, 2021）
- 谷氨酸转运失调与 VEGF 阻断耐药（Cancer Res, 2020）

### 肿瘤微环境与免疫抑制
- CD70 促进胶质瘤迁移与巨噬细胞浸润（IJC, 2017）
- IDH1 突变与 PD-L1 表达/甲基化（Front Mol Neurosci, 2018）

### 转化与临床前研究
- CAR-T 在胶质母细胞瘤体内多模态示踪（Invest Radiol, 2023）
- CAR-T 在实体瘤微环境的运动与功能（Cells, 2022）

---

## 按年份查看

### 詹仁亚 教授
完整列表（111 篇）请见：
[PubMed](https://pubmed.ncbi.nlm.nih.gov/?term=Zhan+Renya%5BAuthor%5D+OR+Zhan+RY%5BAuthor%5D+OR+reyna+zhan%5BAuthor%5D) ｜ [ResearchGate](https://www.researchgate.net/scientific-contributions/Renya-Zhan-14439456)

{% if site.data.publications_zhan %}
{% for year_group in site.data.publications_zhan %}
<div class="year-group">
    <h3 class="year-heading">{{ year_group.year }}</h3>
    {% for pub in year_group.publications %}
    <div class="publication">
        <div class="publication-title">{{ pub.title }}</div>
        <div class="publication-authors">{{ pub.authors }}</div>
        <div class="publication-journal">{{ pub.journal }}</div>
        {% if pub.citations or pub.doi %}
        <div class="publication-meta">
            {% if pub.citations %}<span class="publication-citations">引用：{{ pub.citations }}</span>{% endif %}
            {% if pub.doi %}<span><a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a></span>{% endif %}
        </div>
        {% endif %}
    </div>
    {% endfor %}
</div>
{% endfor %}
{% endif %}

### 金林春 博士
完整列表（152+）请见：
[ResearchGate](https://www.researchgate.net/profile/Linchun-Jin) ｜ [Google Scholar](https://scholar.google.com/citations?user=lyjgFrUAAAAJ&hl=zh-CN)

{% if site.data.publications_jin %}
{% for year_group in site.data.publications_jin %}
<div class="year-group">
    <h3 class="year-heading">{{ year_group.year }}</h3>
    {% for pub in year_group.publications %}
    <div class="publication">
        <div class="publication-title">{{ pub.title }}</div>
        <div class="publication-authors">{{ pub.authors }}</div>
        <div class="publication-journal">{{ pub.journal }}</div>
        {% if pub.citations or pub.doi %}
        <div class="publication-meta">
            {% if pub.citations %}<span class="publication-citations">引用：{{ pub.citations }}</span>{% endif %}
            {% if pub.doi %}<span><a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a></span>{% endif %}
        </div>
        {% endif %}
    </div>
    {% endfor %}
</div>
{% endfor %}
{% endif %}

---

## 专利
- **表达 IL-8 受体的 CAR-T 细胞**  
  J Huang, L Jin  
  US Patent 11,788,093 (2023)

- **乳酸受体工程化 T 细胞**  
  L Deleyrolle, D Mitchell, J Huang, L Jin  
  US Patent App. 18/842,078 (2025)

