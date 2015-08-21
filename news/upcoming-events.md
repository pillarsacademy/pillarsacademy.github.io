---
layout: default
---

# Upcoming Events


<img src="https://cloud.githubusercontent.com/assets/11180395/8606204/0398ea6e-263f-11e5-8a85-3e8e129a4bd1.jpg" width="600" />
{% for event in site.categories['upcoming-events'] reversed %}
  {{ event.date | date: "%D" }} &mdash; [{{ event.title }}]({{ event.url }})
{% endfor %}
