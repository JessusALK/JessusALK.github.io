---
layout: archive
title: Posts

permalink: /posts/
---
<p>
{% for post in site.posts %}
    <h3 class="archive__subtitle"><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p><small><strong>{{ post.date | date: "%B %e, %Y" }}</strong> - {{ post.excerpt | remove: '<p>' | remove: '</p>' }}</small></p>
{% endfor %}
</p>
