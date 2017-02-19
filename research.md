---
layout: page
title: Research
permalink: /research/
---

<strong>Projects</strong>

<ul class="post-list">
{% for post in site.categories['project'] %}
  <li>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

    <h2>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h2>

 	{{ post.content | strip_html | truncatewords:75}}<br>
      <a href="{{ post.url }}">Read more...</a><br>
  </li>

{% endfor %}
</ul>

<strong>News</strong>

<ul class="post-list">
{% for post in site.categories['news'] %}
  <li>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

    <h2>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h2>

 	{{ post.content | strip_html | truncatewords:75}}<br>
      <a href="{{ post.url }}">Read more...</a><br>
  </li>
{% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>