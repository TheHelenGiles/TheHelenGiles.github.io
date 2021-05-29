---
layout: default
title: Blog
permalink: /blog/directory
---
# Directory

{% for tag in site.tags reversed %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li>{{ post.date | date: "%B %e"}}: <i><a href="{{ post.url }}">{{ post.title }}</a></i></li>
    {% endfor %}
  </ul>
{% endfor %}
