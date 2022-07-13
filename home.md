---
layout: page
title: Home
description: Listing of course topics by date.
permalink: /
has_toc: false
nav_order: 1
---

## Momentum Software Engineering Immersive

_Topics are listed by date, newest to oldest._

{% assign modules = site.modules | sort: "phase" | reverse %}

{% for module in modules %}
  {{ module }}
{% endfor %}
