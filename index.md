---
layout: default
title: Home
---

<div class="hero-section" style="background-image: linear-gradient(135deg, rgba(7,75,53,0.82) 0%, rgba(9,105,75,0.82) 50%, rgba(12,122,94,0.82) 100%), url('{{ '/assets/images/Banner.jpg' | relative_url }}');">
    <div class="hero-inner">
        <h1>Zhan/Jin Laboratory</h1>
        <p>Advancing cancer neuroscience and immunotherapy for brain tumors through innovative CAR-T cell engineering and translational research</p>
    </div>
</div>

<div class="home-section">
    <h2>Our Mission</h2>
    <p>Glioblastoma (GBM) remains one of the most devastating brain tumors, with limited treatment options and poor survival rates. Our laboratory focuses on understanding the complex interactions between the immune system and brain tumors, developing novel immunotherapeutic approaches, particularly CAR-T cell therapies, to overcome the immunosuppressive tumor microenvironment and improve patient outcomes.</p>
    
    <p>We integrate cutting-edge cancer neuroscience, cancer immunology, and cellular engineering to tackle fundamental questions about how brain tumors evade immune surveillance and how we can harness the immune system to fight back.</p>
</div>

<div class="home-section research-focus-block">
    <div class="research-text">
        <h2>Research Focus</h2>
        <div class="research-grid">
            <div class="research-area">
                <h3>Cancer Neuroscience</h3>
                <p>Investigating the unique neurobiological features of brain tumors and their microenvironment to identify novel therapeutic targets.</p>
            </div>
            <div class="research-area">
                <h3>Cancer Immunology</h3>
                <p>Understanding immune dysfunction in glioblastoma and developing strategies to enhance anti-tumor immunity.</p>
            </div>
            <div class="research-area">
                <h3>CAR-T Cell Therapy</h3>
                <p>Engineering chimeric antigen receptor T cells with enhanced tumor-targeting, persistence, and efficacy against solid tumors.</p>
            </div>
            <div class="research-area">
                <h3>Glioblastoma Research</h3>
                <p>Characterizing mechanisms of treatment resistance and developing combination therapeutic strategies for GBM.</p>
            </div>
            <div class="research-area">
                <h3>Neuro-oncology</h3>
                <p>Translating laboratory discoveries into clinical applications to improve outcomes for patients with brain tumors.</p>
            </div>
        </div>
    </div>
    <div class="research-visual">
        <img src="{{ '/assets/images/ResearchFocus.jpg' | relative_url }}" alt="Research focus illustration showing glioblastoma immunology and CAR-T therapy">
    </div>
</div>

<div class="home-section">
    <h2>Latest News</h2>
    <ul class="news-list">
    {% for post in site.posts limit:3 %}
        <li class="news-item">
            <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
            <div class="news-date">{{ post.date | date: "%B %d, %Y" }}</div>
            <p class="news-excerpt">{{ post.excerpt }}</p>
        </li>
    {% endfor %}
    </ul>
    <p style="text-align: center; margin-top: 2rem;">
        <a href="{{ '/news/' | relative_url }}" style="font-weight: 500;">View all news →</a>
    </p>
</div>

<div class="home-section">
    <h2>Join Our Team</h2>
    <p>We welcome motivated students, postdoctoral fellows, and visiting scholars with backgrounds in immunology, neuroscience, molecular biology, bioengineering, or related fields. If you are passionate about advancing cancer immunotherapy and making a difference in patients' lives, please reach out to us.</p>
    <p style="text-align: center; margin-top: 1.5rem;">
        <a href="{{ '/contact/' | relative_url }}" style="font-weight: 500; font-size: 1.1rem;">Contact Us →</a>
    </p>
</div>

