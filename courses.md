---
layout: page
title: Courses
permalink: /courses/
---

<ul>
  {% for course in site.data.courses %}
    <li><a href="/courses/{{ course.file }}/">{{ course.name }}</a></li>
  {% endfor %}
</ul>
