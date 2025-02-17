---
layout: page
title: "Projects"
permalink: /projects.html
---

<h1>Projects</h1>
<ul>
  {% for project in site.pages %}
    {% if project.path contains 'projects/' %}
      <li>
        <a href="{{ project.url }}">{{ project.title }}</a>
        <p>{{ project.excerpt }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
