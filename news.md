---
layout: default
title: News
---
Big news
<ul class="blog-items">
{% for post in site.categories.News %}
{% if post.url %}
 <li>
  <a href="{{site.baseurl}}{{post.url}}">
      {{ post.title }} - 
 <time>{{ post.date | date: "%B %d, %Y" }}</time>
</a>
</li>
{% endif %}
{% endfor %}
</ul>