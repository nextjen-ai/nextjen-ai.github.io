---
layout: default
title: Projects
permalink: /projects/
---

<section class="projects-header">
    <h1>Recent AI and GenAI Projects</h1>
</section>

<section class="projects-content">
    <div class="projects-grid">
        {% assign sorted_projects = site.projects | sort: 'order' %}
        {% for project in sorted_projects %}
        <div class="project-card">
            <div class="project-image">
                <img src="{{ project.image | default: '/assets/images/placeholder.jpg' }}" alt="{{ project.title }}">
            </div>
            <div class="project-content">
                <h2>{{ project.title }}</h2>
                <div class="project-tags">
                    {% for tag in project.tags %}
                    <span class="tag">{{ tag }}</span>
                    {% endfor %}
                </div>
                {{ project.content | markdownify }}
            </div>
        </div>
        {% endfor %}
    </div>
</section>

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
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
}

.project-card:hover {
    transform: translateY(-5px);
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

@media (max-width: 768px) {
    .projects-content {
        padding: 2rem 1rem;
    }
    
    .projects-header {
        padding: 3rem 1rem;
    }
}
</style> 