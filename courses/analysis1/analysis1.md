---
layout: course_page
title: Analysis 1
categories: sem1
use_latex : true
permalink: /courses/analysis1/
---

{% assign set_pages = site.pages | select: "layout", "set" %}
{% assign folder_name = page.permalink | split: '/' | slice: - %}
{{folder_name}}
{% assign filtered_pages = set_pages | select: "permalink", "/courses/" | append: folder_name %}

{% for page in filtered_pages %}
  <li><a href="{{ page.url | relative_url }}">{{ page.title }}</a></li>
{% endfor %}



$$f(x) = \{x \in S \mid y \in K \land (x, y) \in B \}$$

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
