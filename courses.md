---
layout: header_page
title: Courses
permalink: /courses
---

<ul>
  {% assign course_pages = site.pages | where_exp: "page", "page.url contains '/courses/'" %}
  {% for course in course_pages %}
    <li><a href="{{ course.url | relative_url }}">{{ course.title }}</a></li>
  {% endfor %}
</ul>
