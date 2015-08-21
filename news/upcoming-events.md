---
layout: default
---

# Upcoming Events


{% for event in site.categories['upcoming-events'] reversed %}
  {{ event.date | date: "%D" }} &mdash; [{{ event.title }}]({{ event.url }})
{% endfor %}
