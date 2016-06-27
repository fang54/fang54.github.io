---
layout: page
title: fang的家园
tagline: 那个让你刻苦铭心的名字始终不是我。
---
{% include JB/setup %}
 
你好，世界！


<ul>

　　{% for post in site.posts %}

　　　　<li>{{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
            <p> {{ post.content  | | split:'<!--break-->' | first }}</p>

　　{% endfor %}

</ul>
