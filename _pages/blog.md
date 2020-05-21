---
layout: page
title: Blog
permalink: /blog/
---

## {{ page.title }}

<ul class="post-list">
{% for post in site.categories['blog'] %}
  <li>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

    <h2>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h2>

 	{{ post.content | strip_html | truncatewords:50}}<br>
      <a href="{{ post.url }}">Read more...</a><br>
  </li>

{% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>

back to [home][1]

[1]: {{ site.baseurl }}{% link index.md %}