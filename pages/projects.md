---
permalink: /projects.html
layout: default
title: CLARIPHY Projects
---

# Projects involving CLARIPHY collaborators

<ul>
{% assign sorted = site.pages | sort_natural: 'title' %}
{% for mypage in sorted %}
{% if mypage.layout == 'project' %} 
  <li><a href="{{mypage.permalink}}">{{ mypage.title }}</a> - {{ mypage.description }} </li>
{% endif %}
{% endfor %}
</ul>
