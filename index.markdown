---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Welcome
order: 1
layout: home
minima:
  social_links:
    github: ron2015schmitt
---


Hello and welcome to my site!  I am a software developer with extensive experience, who likes clean well-designed code.  This site highlights some of my personal and independent projects, as well as my skill set.

{% assign sorted_pages = site.pages | sort:"order" %}
{% for page in sorted_pages %}
  {% if page.title and page.title != "Welcome" %}
* [{{ page.title }}]({{ page.url }}) 
  {% endif %}
{% endfor %}
