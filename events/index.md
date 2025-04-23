---
layout: default
title: Upcoming Events
---

# Upcoming Events

{% for event in site.events %}
<div class="card mb-4">
    <div class="card-body">
        <h2 class="card-title">{{ event.title }}</h2>
        <p class="text-muted">
            Date: {{ event.date | date: "%B %d, %Y" }}<br>
            Location: {{ event.location }}
        </p>
        <div class="card-text">
            {{ event.description }}
        </div>
        <a href="{{ event.url | relative_url }}" class="btn btn-primary">View Details</a>
    </div>
</div>
{% endfor %} 