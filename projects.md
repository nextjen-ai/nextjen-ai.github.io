---
layout: default
title: Projects
permalink: /projects/
---

{% include projects-content.html %}

<style>
.projects-header {
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    color: var(--white);
    padding: 4rem 0;
    text-align: center;
}

.projects-header h1 {
    color: var(--white);
    margin: 0;
}

.projects-content {
    max-width: 1200px;
    margin: 0 auto;
    padding: 4rem 2rem;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

.project-card {
    background: var(--white);
    border-radius: 8px;
    overflow: hidden;
    transition: border-color 0.3s ease;
}

.project-card:hover {
    border: 1px solid var(--secondary-color);
}

.project-image {
    width: 100%;
    height: 200px;
    overflow: hidden;
}

.project-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.project-content {
    padding: 1.5rem;
}

.project-content h2 {
    color: var(--primary-color);
    margin-bottom: 1rem;
    font-size: 1.5rem;
}

.project-content h3 {
    color: var(--primary-color);
    margin: 1rem 0 0.5rem 0;
    font-size: 1.2rem;
}

.project-tags {
    margin-bottom: 1rem;
}

.tag {
    display: inline-block;
    background: var(--light-gray);
    color: var(--primary-color);
    padding: 0.25rem 0.75rem;
    border-radius: 15px;
    font-size: 0.875rem;
    margin-right: 0.5rem;
    margin-bottom: 0.5rem;
}

.project-content ul {
    list-style-type: none;
    padding-left: 0;
}

.project-content li {
    margin-bottom: 0.5rem;
    position: relative;
    padding-left: 1.2rem;
}

.project-content li:before {
    content: "•";
    color: var(--secondary-color);
    position: absolute;
    left: 0;
}

@media (max-width: 768px) {
    .projects-content {
        padding: 2rem 1rem;
    }
    
    .projects-header {
        padding: 3rem 1rem;
    }
}
</style> 