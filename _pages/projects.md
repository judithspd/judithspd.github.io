---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

{% assign project_documents = site.projects.docs | default: site.projects %}
{% assign international_projects = project_documents | where: "scope", "International" | sort: "display_order" %}
{% assign national_projects = project_documents | where: "scope", "National" | sort: "date" | reverse %}

<h2 style="margin-bottom: 1rem; border-bottom: 2px solid #7a003c; padding-bottom: 0.4rem; letter-spacing: 0.01em;">Participation and leadership in international projects</h2>

{% for post in international_projects %}
  <div class="project-card" style="margin-bottom: 1.25rem; padding: 1.1rem 1.2rem; border: 1px solid #e5d8df; border-left: 6px solid #7a003c; background: linear-gradient(90deg, #fcf7fa 0%, #ffffff 100%); box-shadow: 0 1px 3px rgba(0,0,0,0.06);">
    <div class="project-card__layout">
      {% if post.logo %}<a class="project-card__logo" href="{{ post.website | default: post.url | relative_url }}"{% if post.website %} target="_blank" rel="noopener noreferrer"{% endif %}><img src="{% if post.logo contains '://' %}{{ post.logo }}{% else %}{{ post.logo | prepend: '/images/' | prepend: base_path }}{% endif %}" alt="{{ post.title }} logo"></a>{% endif %}
      <div class="project-card__body">
    <h3>
      {% if post.website %}
        <a href="{{ post.website }}" target="_blank" rel="noopener noreferrer">{{ post.title }}</a>
      {% else %}
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      {% endif %}
    </h3>
    <p><strong>Type:</strong> {{ post.scope | default: "International" }}</p>
    <p><strong>Funding:</strong> {{ post.funding | default: post.funding_source | default: "Not disclosed" }}</p>
    <p><strong>Duration:</strong> {{ post.duration | default: "Not available" }}</p>
    <p><strong>Budget:</strong> {{ post.total_funding | default: post.budget | default: "Not disclosed" }}</p>
    <p><strong>Coordinator:</strong> {{ post.coordinator | default: "Not specified" }}</p>
    {% if post.role %}
      <p><strong>Role:</strong> <span style="color:#7a003c; font-weight:700;">{{ post.role }}</span></p>
    {% endif %}
    {% if post.main_tasks %}
      <p><strong>Main tasks:</strong> {{ post.main_tasks }}</p>
    {% endif %}
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% endif %}
      </div>
    </div>
  </div>
{% endfor %}

<h2 style="margin-bottom: 1rem; border-bottom: 2px solid #4c6ef5; padding-bottom: 0.4rem; letter-spacing: 0.01em;">Participation in competitive national projects</h2>

{% for post in national_projects %}
  <div class="project-card" style="margin-bottom: 1.25rem; padding: 1.1rem 1.2rem; border: 1px solid #dfe6f7; border-left: 6px solid #4c6ef5; background: linear-gradient(90deg, #f7faff 0%, #ffffff 100%); box-shadow: 0 1px 3px rgba(0,0,0,0.06);">
    <div class="project-card__layout">
      {% if post.logo %}<a class="project-card__logo" href="{{ post.website | default: post.url | relative_url }}"{% if post.website %} target="_blank" rel="noopener noreferrer"{% endif %}><img src="{% if post.logo contains '://' %}{{ post.logo }}{% else %}{{ post.logo | prepend: '/images/' | prepend: base_path }}{% endif %}" alt="{{ post.title }} logo"></a>{% endif %}
      <div class="project-card__body">
    <h3>
      {% if post.website %}
        <a href="{{ post.website }}" target="_blank" rel="noopener noreferrer">{{ post.title }}</a>
      {% else %}
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      {% endif %}
    </h3>
    <p><strong>Type:</strong> {{ post.scope | default: "National" }}</p>
    <p><strong>Funding:</strong> {{ post.funding | default: post.funding_source | default: "Not disclosed" }}</p>
    <p><strong>Duration:</strong> {{ post.duration | default: "Not available" }}</p>
    <p><strong>Budget:</strong> {{ post.total_funding | default: post.budget | default: "Not disclosed" }}</p>
    <p><strong>Coordinator:</strong> {{ post.coordinator | default: "Not specified" }}</p>
    {% if post.role %}
      <p><strong>Role:</strong> <span style="color:#4c6ef5; font-weight:700;">{{ post.role }}</span></p>
    {% endif %}
    {% if post.main_tasks %}
      <p><strong>Main tasks:</strong> {{ post.main_tasks }}</p>
    {% endif %}
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% endif %}
      </div>
    </div>
  </div>
{% endfor %}
