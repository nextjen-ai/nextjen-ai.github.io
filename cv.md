---
layout: default
title: CV
permalink: /cv/
---

<div class="cv-page">
    <div class="cv-header">
        <h1>Jennifer Andreoli-Fang, PhD</h1>
        <p class="cv-subtitle">Software Engineer & AI Enthusiast</p>
    </div>

    <div class="cv-content">
        {% include cv-content.html %}
    </div>
</div>

<style>
.cv-page {
    max-width: 900px;
    margin: 0 auto;
    padding: 1.5rem;
}

.cv-header {
    text-align: center;
    margin-bottom: 2rem;
}

.cv-subtitle {
    color: var(--secondary-color);
    font-size: 1.2rem;
    margin-top: 0.3rem;
}

.cv-section {
    margin-bottom: 2rem;
}

.cv-section h2 {
    color: var(--primary-color);
    font-size: 1.6rem;
    margin-bottom: 1rem;
    border-bottom: 2px solid var(--secondary-color);
    padding-bottom: 0.3rem;
}

.cv-section h3 {
    color: var(--primary-color);
    margin: 1.2rem 0 0.3rem 0;
    font-size: 1.3rem;
}

.cv-section h4 {
    color: var(--text-color);
    font-weight: 400;
    margin: 0 0 0.5rem 0;
    font-size: 1.1rem;
}

.cv-section ul {
    list-style-type: none;
    padding-left: 0;
    margin-bottom: 0.5rem;
}

.cv-section li {
    margin-bottom: 0.4rem;
    position: relative;
    padding-left: 1.2rem;
    line-height: 1.4;
}

.cv-section li:before {
    content: "•";
    color: var(--secondary-color);
    position: absolute;
    left: 0;
}

.cv-section p {
    margin-bottom: 0.5rem;
    line-height: 1.4;
}

.cv-section em {
    color: var(--secondary-color);
    font-style: normal;
}

@media (max-width: 768px) {
    .cv-page {
        padding: 1rem;
    }
}
</style> 