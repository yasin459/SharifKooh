---
layout: default
title: Climbing Calendar
---

# Climbing Calendar

{% for entry in site.calendar %}
<div class="card mb-4">
    <div class="card-body">
        <h2 class="card-title">{{ entry.title }}</h2>
        <p class="text-muted">
            Date: {{ entry.date | date: "%B %d, %Y" }}<br>
            Location: {{ entry.location }}
        </p>
        <div class="card-text">
            {{ entry.description }}
        </div>
        <a href="{{ entry.url | relative_url }}" class="btn btn-primary">View Details</a>
    </div>
</div>
{% endfor %} 