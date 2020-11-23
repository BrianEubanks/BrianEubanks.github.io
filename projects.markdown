---
layout: page
title: Projects
permalink: /projects/
---

List of Projects.

<ul>
  {% for post in site.posts %}
    {% if post.project == 'CS' %}
        <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        </li>
    {% endif %}
  {% endfor %}
</ul>


