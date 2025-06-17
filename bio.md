---
layout: default
title: About Me
permalink: /bio/
---

<div class="bio-page">
    <div class="bio-header">
        <h1>About Me</h1>
        <p class="bio-subtitle">Technology Leader & AI Builder</p>
    </div>

    <div class="bio-content">
        {% assign bio_sections = site.bio | sort: 'order' %}
        {% for section in bio_sections %}
        <section class="bio-section">
            <h2>{{ section.title }}</h2>
            {{ section.content | markdownify }}
        </section>
        {% endfor %}
    </div>
</div>

<style>
.bio-page {
    max-width: 800px;
    margin: 0 auto;
    padding: 2rem;
}

.bio-header {
    text-align: center;
    margin-bottom: 4rem;
}

.bio-subtitle {
    color: var(--secondary-color);
    font-size: 1.2rem;
    margin-top: 1rem;
}

.bio-section {
    margin-bottom: 3rem;
}

.bio-section h2 {
    color: var(--primary-color);
    font-size: 1.8rem;
    margin-bottom: 1.5rem;
}

.bio-section p {
    font-size: 1.1rem;
    line-height: 1.8;
    color: var(--text-color);
}

@media (max-width: 768px) {
    .bio-page {
        padding: 1rem;
    }
    
    .bio-header {
        margin-bottom: 2rem;
    }
    
    .bio-section {
        margin-bottom: 2rem;
    }
}
</style> 