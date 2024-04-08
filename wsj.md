---
title: ⓌⓈⒿ
layout: page
permalink: /wsj/
---
{% for category in site.categories %}
  {% if category.first == "wsj" %}
  <div>
    {% for post in category.last %}
    <span class="postdate">{{ post.date | preserve_timezones }}</span> • <span class="author">WSJ</span>
    <h4><a href="{{site.url}}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h4>
    {% endfor %}
  </div>
  {% endif %}
{% endfor %}

