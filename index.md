---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Hyperlinks to each of the lab exercises and demos are listed below.

## Exercise Secure-Networking

{% assign Exercise = site.pages | where_exp:"page", "page.url contains '/Secure-Networking/Exercises'" %}
| Module | Exercise |
| --- | --- | 
{% for activity in Exercise  %}| {{ activity.Exercise.module }} | [{{ activity.Exercise.title }}{% if activity.Exercise.type %} - {{ activity.Exercise.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

## Exercise Secure-Storage 

{% assign Exercise = site.pages | where_exp:"page", "page.url contains '/Secure storage/Exercises'" %}
| Module | Exercise |
| --- | --- | 
{% for activity in Exercise  %}| {{ activity.Exercise.module }} | [{{ activity.Exercise.title }}{% if activity.Exercise.type %} - {{ activity.Exercise.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
