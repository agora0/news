---
title: 🅱🅱🅲
layout: page
category: ["bbc","nyt"]
permalink: /bbc/
---
{% for category in site.categories %}
  {% if category.first == page.category[0] %}
    {% assign category_0 = category %}
  {% elsif category.first == page.category[1] %}
    {% assign category_1 = category %}
  {% endif %} 
{% endfor %}
{% assign posts = category_0.last | concat: category_1.last | sort: "date" | reverse %}
<div>
{% for post in posts %}
  <span class="postdate">{{ post.date | preserve_timezones }}</span> • <span class="author"><a href="{{ site.url }}{{ site.baseurl }}/{{ post.categories }}">{{ post.categories.first | upcase }}</a></span>
  <h4><a href="{{site.url}}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h4>
{% endfor %}
</div>

