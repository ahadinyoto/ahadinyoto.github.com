---
layout: page
title: Andrew's blog!
---
{% include JB/setup %}

{{ site.posts.last.content }}


<hr>

<h3>Other posts</h3>

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

