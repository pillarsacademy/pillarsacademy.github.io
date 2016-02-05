---
layout: default
---

# [Upcoming Events](http://www.pillarsacademy.org/)


{% for event in site.categories['upcoming-events'] reversed %}
  {{ event.date | date: "%D" }} &mdash; [{{ event.title }}]({{ event.url }})
{% endfor %}
