---
layout: page
permalink: /blog/
title: blog
description: Showcase your writing, short stories, or poems. Replace this text with your description.
---

<ul class="post-list">
{% for poem in site.poetry reversed %}
    <li>
        <h2><a class="blog-title" href="{{ blog.url | prepend: site.baseurl }}">{{ blog.title }}</a></h2>
        <p class="post-meta">{{ blog.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
