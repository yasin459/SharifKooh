---
layout: default
title: Trip Reports
---

# Trip Reports

{% for report in site.reports %}
<div class="card mb-4">
    <div class="card-body">
        <h2 class="card-title">{{ report.title }}</h2>
        <p class="text-muted">
            Date: {{ report.date | date: "%B %d, %Y" }}<br>
            Location: {{ report.location }}<br>
            Participants: {{ report.participants }}
        </p>
        <a href="{{ report.url | relative_url }}" class="btn btn-primary">Read Report</a>
    </div>
</div>
{% endfor %} 