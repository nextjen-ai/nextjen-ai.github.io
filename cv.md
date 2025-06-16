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
        <section class="cv-section">
            <h2>Summary</h2>
            <p>{{ site.data.cv.summary }}</p>
            
            <ul class="cv-highlights">
                {% for highlight in site.data.cv.highlights %}
                <li>{{ highlight }}</li>
                {% endfor %}
            </ul>

            <p class="cv-patents">{{ site.data.cv.patents }}</p>
        </section>

        <section class="cv-section">
            <h2>Professional Experience</h2>
            {% for job in site.data.cv.experience %}
            <div class="cv-job">
                <div class="cv-job-header">
                    <h3>{{ job.company }}</h3>
                    <span class="cv-period">{{ job.period }}</span>
                </div>
                <h4>{{ job.title }}</h4>
                <ul class="cv-achievements">
                    {% for achievement in job.achievements %}
                    <li>{{ achievement }}</li>
                    {% endfor %}
                </ul>
            </div>
            {% endfor %}
        </section>

        <section class="cv-section">
            <h2>Awards & Recognition</h2>
            <ul class="cv-awards">
                {% for award in site.data.cv.awards %}
                <li>{{ award }}</li>
                {% endfor %}
            </ul>
        </section>

        <section class="cv-section">
            <h2>Education</h2>
            {% for edu in site.data.cv.education %}
            <div class="cv-education">
                <h3>{{ edu.degree }}</h3>
                {% if edu.school %}
                <p class="cv-school">{{ edu.school }}</p>
                {% endif %}
                {% if edu.details %}
                <p class="cv-details">{{ edu.details }}</p>
                {% endif %}
                <p class="cv-year">{{ edu.year }}</p>
            </div>
            {% endfor %}
        </section>

        <section class="cv-section">
            <h2>Get in Touch</h2>
            <div class="cv-contact">
                <a href="mailto:{{ site.data.cv.contact.email }}" class="cv-contact-link">
                    <i class="fas fa-envelope"></i> {{ site.data.cv.contact.email }}
                </a>
                <a href="{{ site.data.cv.contact.linkedin }}" class="cv-contact-link" target="_blank">
                    <i class="fab fa-linkedin"></i> LinkedIn
                </a>
            </div>
        </section>
    </div>
</div>

<style>
.cv-page {
    max-width: 900px;
    margin: 0 auto;
    padding: 2rem;
}

.cv-header {
    text-align: center;
    margin-bottom: 3rem;
}

.cv-subtitle {
    color: var(--secondary-color);
    font-size: 1.2rem;
    margin-top: 0.5rem;
}

.cv-section {
    margin-bottom: 3rem;
}

.cv-section h2 {
    color: var(--primary-color);
    font-size: 1.8rem;
    margin-bottom: 1.5rem;
    border-bottom: 2px solid var(--secondary-color);
    padding-bottom: 0.5rem;
}

.cv-highlights {
    list-style-type: none;
    padding-left: 0;
}

.cv-highlights li {
    margin-bottom: 0.8rem;
    position: relative;
    padding-left: 1.5rem;
}

.cv-highlights li:before {
    content: "•";
    color: var(--secondary-color);
    position: absolute;
    left: 0;
}

.cv-patents {
    font-style: italic;
    margin-top: 1.5rem;
}

.cv-job {
    margin-bottom: 2rem;
}

.cv-job-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 0.5rem;
}

.cv-job h3 {
    color: var(--primary-color);
    margin: 0;
}

.cv-period {
    color: var(--secondary-color);
    font-size: 0.9rem;
}

.cv-job h4 {
    color: var(--text-color);
    font-weight: 400;
    margin: 0 0 1rem 0;
}

.cv-achievements {
    list-style-type: none;
    padding-left: 0;
}

.cv-achievements li {
    margin-bottom: 0.8rem;
    position: relative;
    padding-left: 1.5rem;
}

.cv-achievements li:before {
    content: "•";
    color: var(--secondary-color);
    position: absolute;
    left: 0;
}

.cv-awards {
    list-style-type: none;
    padding-left: 0;
}

.cv-awards li {
    margin-bottom: 0.8rem;
    position: relative;
    padding-left: 1.5rem;
}

.cv-awards li:before {
    content: "•";
    color: var(--secondary-color);
    position: absolute;
    left: 0;
}

.cv-education {
    margin-bottom: 1.5rem;
}

.cv-education h3 {
    color: var(--primary-color);
    margin: 0;
}

.cv-school {
    color: var(--text-color);
    margin: 0.3rem 0;
}

.cv-details {
    color: var(--text-color);
    font-style: italic;
    margin: 0.3rem 0;
}

.cv-year {
    color: var(--secondary-color);
    margin: 0.3rem 0;
}

.cv-contact {
    display: flex;
    gap: 2rem;
    justify-content: center;
    margin-top: 1rem;
}

.cv-contact-link {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    color: var(--secondary-color);
    text-decoration: none;
    transition: color 0.3s ease;
}

.cv-contact-link:hover {
    color: var(--primary-color);
}

@media (max-width: 768px) {
    .cv-page {
        padding: 1rem;
    }
    
    .cv-job-header {
        flex-direction: column;
        gap: 0.5rem;
    }
    
    .cv-contact {
        flex-direction: column;
        align-items: center;
        gap: 1rem;
    }
}
</style> 