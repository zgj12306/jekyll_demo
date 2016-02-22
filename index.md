---
layout: default
title: 我的Blog
---
<h2>{{ page.title }}</h2>
<p>最新文章</p>
<ul>
  {% for post in site.posts %}
  <li>
    <a href="{{ site.baseurl }}{{ post.url }}">
     {{ post.title }}
    </a>
    {{ post.date | date_to_string }}
  </li>
  {% endfor %}
</ul>
  
