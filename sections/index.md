---
layout: default
title: Group Sections
---

# Group Sections

{% for section in site.sections %}
<div class="card mb-4">
    <div class="card-body">
        <h2 class="card-title">{{ section.title }}</h2>
        <p class="text-muted">{{ section.description }}</p>
        {% if section.members %}
        <p><strong>Members:</strong> {{ section.members }}</p>
        {% endif %}
        <a href="{{ section.url | relative_url }}" class="btn btn-primary">View Section</a>
    </div>
</div>
{% endfor %} 