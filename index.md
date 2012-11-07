---
layout: page
title: gelgels
tagline: los angeles native | ucla computer science | tech enthusiast
---
{% include JB/setup %}


<ul class="posts">
  {% for post in site.posts %}
    <li>
      <span>
        {{ post.date | date_to_string }}
      </span> &raquo;
      <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
      {{ post.content | strip_html | truncatewords:100 }}
    </li>
  {% endfor %}
</ul>


