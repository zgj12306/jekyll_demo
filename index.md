---
layout: default
title: 我的Blog
---
## {{ page.title }}
{% for post in site.post offset: 0 limit: 10 %}
	<h2>
        <a href="{{ site.prefix }}{{ post.url }}">{{ post.title }}</a>
    </h2>  
    {{ post.content }}
    {{ post.date | date_to_string }}
    <hr />
{% endfor %}
{% include about.md %}

