---
layout: default
title: Home
---

# Welcome to {{ site.title }}

We are a community of mountain enthusiasts who share the passion for climbing and outdoor adventures.

## Latest Trip Reports

{% for report in site.reports limit:3 %}
- [{{ report.title }}]({{ report.url | relative_url }}) - {{ report.date | date: "%B %d, %Y" }}
{% endfor %}

## Upcoming Events

{% for event in site.events limit:3 %}
- [{{ event.title }}]({{ event.url | relative_url }}) - {{ event.date | date: "%B %d, %Y" }}
{% endfor %}

## Join Our Community

We welcome new members who share our passion for mountaineering. Check out our [About](/about) page to learn more about our group and how to get involved. 