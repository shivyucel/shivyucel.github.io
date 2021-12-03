---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home-projects
title: "Projects"
category: "projects"
weight: 2
---
<ul>
  {% for post in projects.posts %}
    {% if post.docurl %}
      <li><a href="{{ projects.baseurl }}{{ projects.docurl }}">{{ post.title }}</a></li>
    {% else %}
      <li><a href="{{ projects.baseurl }}{{ projects.url }}">{{ post.title }}</a></li>
    {% endif %}
    {{ post.excerpt }}
  {% endfor %}
</ul>