---
layout: home
title: General Posts
permalink: posts/index.html
nav_order: 2
---

## Announcements

This page is for occasional updates and general information.

**Daily topics** are on the [home page]({% link home.md %}), along with links to **course material**, **resources**, and **lab assignments**.
{: .pb-3 .announcement-detail }

{% assign general_posts = site.general_posts | reverse %}
{% for post in general_posts %}
{{ post }}
{% endfor %}
