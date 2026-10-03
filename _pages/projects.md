---
layout: page
title: projects
permalink: /projects/
description: Selected software and applied AI projects.
nav: true
published: true
nav_order: 2
horizontal: true
---

These projects reflect my interests in applied artificial intelligence, information retrieval, data visualization, computational finance, and human-centered digital systems. Source code and fuller technical documentation are available on [my GitHub profile](https://github.com/XINGYI-PU).

{% assign sorted_projects = site.projects | sort: 'importance' %}

<ol class="project-list">
  {% for project in sorted_projects %}
    <li class="project-entry">
      <div class="project-category">{{ project.category | replace: '-', ' ' }}</div>
      <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
      <p>{{ project.description }}</p>
      <div class="project-links">
        <a href="{{ project.url | relative_url }}">Project details <span aria-hidden="true">&rarr;</span></a>
        {% if project.github %}<a href="{{ project.github }}">GitHub <span aria-hidden="true">↗</span></a>{% endif %}
      </div>
    </li>
  {% endfor %}
</ol>
