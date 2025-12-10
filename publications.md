---
layout: page
title: Publications
subtitle: Our research contributions to cancer immunotherapy and neuro-oncology
---

Our laboratory has published extensively in high-impact journals, advancing the understanding of brain tumor immunology and developing novel therapeutic approaches. Below are selected publications grouped by principal investigator.

---

## Selected Key Publications

### CAR-T Cell Therapy & Immunotherapy

<div class="publication">
    <div class="publication-title">CXCR1- or CXCR2-modified CAR T cells co-opt IL-8 for maximal antitumor efficacy in solid tumors</div>
    <div class="publication-authors">L Jin, H Tao, A Karachi, Y Long, AY Hou, M Na, KA Dyson, AJ Grippin, et al.</div>
    <div class="publication-journal">Nature Communications 10 (1), 4016</div>
    <div class="publication-meta">
        <span class="publication-year">2019</span>
        <span class="publication-citations">Cited by: 320+</span>
    </div>
</div>

<div class="publication">
    <div class="publication-title">CD70, a novel target of CAR T-cell therapy for gliomas</div>
    <div class="publication-authors">L Jin, H Ge, Y Long, C Yang, Y Chang, L Mu, EJ Sayour, G De Leon, et al.</div>
    <div class="publication-journal">Neuro-Oncology 20 (1), 55-65</div>
    <div class="publication-meta">
        <span class="publication-year">2018</span>
        <span class="publication-citations">Cited by: 209</span>
    </div>
</div>

### Glioblastoma Biology & Resistance Mechanisms

<div class="publication">
    <div class="publication-title">Glioblastoma multiforme (GBM): An overview of current therapies and mechanisms of resistance</div>
    <div class="publication-authors">W Wu, JL Klockow, M Zhang, F Lafortune, E Chang, L Jin, Y Wu, et al.</div>
    <div class="publication-journal">Pharmacological Research 171, 105780</div>
    <div class="publication-meta">
        <span class="publication-year">2021</span>
        <span class="publication-citations">Cited by: 604+</span>
    </div>
</div>

<div class="publication">
    <div class="publication-title">Dysregulation of glutamate transport enhances Treg function that promotes VEGF blockade resistance in glioblastoma</div>
    <div class="publication-authors">Y Long, H Tao, A Karachi, AJ Grippin, L Jin, Y Chang, W Zhang, et al.</div>
    <div class="publication-journal">Cancer Research 80 (3), 499-509</div>
    <div class="publication-meta">
        <span class="publication-year">2020</span>
        <span class="publication-citations">Cited by: 106</span>
    </div>
</div>

### Tumor Microenvironment & Immunosuppression

<div class="publication">
    <div class="publication-title">Tumor associated CD70 expression is involved in promoting tumor migration and macrophage infiltration in GBM</div>
    <div class="publication-authors">H Ge, L Mu, L Jin, C Yang, Y Chang, Y Long, G DeLeon, L Deleyrolle, et al.</div>
    <div class="publication-journal">International Journal of Cancer 141 (7), 1434-1444</div>
    <div class="publication-meta">
        <span class="publication-year">2017</span>
        <span class="publication-citations">Cited by: 88</span>
    </div>
</div>

<div class="publication">
    <div class="publication-title">The IDH1 mutation-induced oncometabolite, 2-hydroxyglutarate, may affect DNA methylation and expression of PD-L1 in gliomas</div>
    <div class="publication-authors">L Mu, Y Long, C Yang, L Jin, H Tao, H Ge, YE Chang, A Karachi, et al.</div>
    <div class="publication-journal">Frontiers in Molecular Neuroscience 11, 82</div>
    <div class="publication-meta">
        <span class="publication-year">2018</span>
        <span class="publication-citations">Cited by: 93</span>
    </div>
</div>

### Translational & Clinical Studies

<div class="publication">
    <div class="publication-title">Multimodal in vivo tracking of chimeric antigen receptor T cells in preclinical glioblastoma models</div>
    <div class="publication-authors">WE Wu, E Chang, L Jin, S Liu, CH Huang, R Kamal, T Liang, NM Aissaoui, et al.</div>
    <div class="publication-journal">Investigative Radiology 58 (6), 388-395</div>
    <div class="publication-meta">
        <span class="publication-year">2023</span>
        <span class="publication-citations">Cited by: 18</span>
    </div>
</div>

<div class="publication">
    <div class="publication-title">CAR T cell locomotion in solid tumor microenvironment</div>
    <div class="publication-authors">DT Nguyen, E Ogando-Rivas, R Liu, T Wang, J Rubin, L Jin, H Tao, et al.</div>
    <div class="publication-journal">Cells 11 (12), 1974</div>
    <div class="publication-meta">
        <span class="publication-year">2022</span>
        <span class="publication-citations">Cited by: 44</span>
    </div>
</div>

---

## Publications by Year

### Professor Zhan Renya

For a complete list of Professor Zhan's publications (111 papers), please see [PubMed](https://pubmed.ncbi.nlm.nih.gov/?term=Zhan+Renya%5BAuthor%5D+OR+Zhan+RY%5BAuthor%5D+OR+reyna+zhan%5BAuthor%5D) and [ResearchGate](https://www.researchgate.net/scientific-contributions/Renya-Zhan-14439456). Selected recent publications include:

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
            {% if pub.citations %}<span class="publication-citations">Cited by: {{ pub.citations }}</span>{% endif %}
            {% if pub.doi %}<span><a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a></span>{% endif %}
        </div>
        {% endif %}
    </div>
    {% endfor %}
</div>
{% endfor %}
{% endif %}

### Dr. Jin Linchun

For a complete list of Dr. Jin's publications (152 entries), please see [ResearchGate](https://www.researchgate.net/profile/Linchun-Jin) and [Google Scholar](https://scholar.google.com/citations?user=lyjgFrUAAAAJ&hl=en). Selected recent publications include:

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
            {% if pub.citations %}<span class="publication-citations">Cited by: {{ pub.citations }}</span>{% endif %}
            {% if pub.doi %}<span><a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a></span>{% endif %}
        </div>
        {% endif %}
    </div>
    {% endfor %}
</div>
{% endfor %}
{% endif %}

---

## Patents

- **Chimeric antigen receptor T-cells expressing interleukin-8 receptor**  
  J Huang, L Jin  
  US Patent 11,788,093 (2023)

- **Chimeric lactate receptor engineered T cells**  
  L Deleyrolle, D Mitchell, J Huang, L Jin  
  US Patent App. 18/842,078 (2025)

---

*Note: This page shows selected publications. Complete publication data will be populated from YAML data files. Citations counts are approximate and may not reflect the most current numbers.*

