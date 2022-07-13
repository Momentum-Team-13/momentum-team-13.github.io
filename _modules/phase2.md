---
title: Phase 2 Back End
phase: 2
---

{% assign topics = site.data.phase2_topics | reverse %}


{% for topic in topics %}
  {{ topic.date | date: "%B %-d" }}
  : [{{ topic.title }}]({% link {{topic.url}} %})
    : [Lab]({{ topic.lab_url }}){: .label .lab-label } [Resources]({% link {{ topic.resources_url }} %}){: .label .resources-label }
{% endfor %}


