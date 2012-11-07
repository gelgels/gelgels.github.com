---
layout: page
title: gelgels
tagline: los angeles native | ucla computer science | tech enthusiast
---
{% include JB/setup %}


<div class="post_container">
  {% for post in site.posts %}
    <div class="post">
      <h2 style="display:inline">
        <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
      </h2>
      &raquo;
      <span> {{ post.date | date_to_string }} </span>
      <br>
      {{ post.content | strip_html | truncatewords:100 }}
    </div>
  {% endfor %}
</div>

