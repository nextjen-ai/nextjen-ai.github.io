---
layout: default
title: Publications
permalink: /publications/
---

{% include publications-content.html %}

<style>
.publications-header {
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    color: var(--white);
    padding: 4rem 0;
    text-align: center;
}

.publications-header h1 {
    color: var(--white);
    margin: 0;
}

.publications-content {
    max-width: 1200px;
    margin: 0 auto;
    padding: 4rem 2rem;
}

.publications-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 2rem;
}

.publication-card {
    background: var(--white);
    border-radius: 8px;
    overflow: hidden;
    transition: border-color 0.3s ease;
}

.publication-card:hover {
    border: 1px solid var(--secondary-color);
}

.publication-content {
    padding: 2rem;
}

.publication-content h2 {
    color: var(--primary-color);
    margin-bottom: 1.5rem;
    font-size: 1.8rem;
    border-bottom: 2px solid var(--secondary-color);
    padding-bottom: 0.5rem;
}

.publication-content h3 {
    color: var(--primary-color);
    margin: 1.5rem 0 0.5rem 0;
    font-size: 1.3rem;
}

.publication-content ul {
    list-style-type: none;
    padding-left: 0;
}

.publication-content li {
    margin-bottom: 0.75rem;
    position: relative;
    padding-left: 1.5rem;
    line-height: 1.6;
}

.publication-content li:before {
    content: "•";
    color: var(--secondary-color);
    position: absolute;
    left: 0;
    font-weight: bold;
}

.publication-content a {
    color: var(--secondary-color);
    text-decoration: none;
    font-weight: 500;
}

.publication-content a:hover {
    text-decoration: underline;
}

@media (max-width: 768px) {
    .publications-content {
        padding: 2rem 1rem;
    }
    
    .publications-header {
        padding: 3rem 1rem;
    }
    
    .publication-content {
        padding: 1.5rem;
    }
}
</style> 