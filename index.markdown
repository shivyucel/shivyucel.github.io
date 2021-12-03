---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# get about page in Here
# {% assign about = site.pages | where: 'name','about.markdown' %}
# {{about}}
layout: default
---

<br/><br/><br/><br/>

## My name is Shiv Yucel and I am a recent graduate of the Social Data Science MSc from the Oxford Internet Institute.


<ul>
  {% for post in site.posts %}
    {% if post.docurl %}
      <li><a href="{{ site.baseurl }}{{ post.docurl }}">{{ post.title }}</a></li>
    {% else %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
    {{ post.excerpt }}
  {% endfor %}
</ul>

