---
title: "Home"
keywords: homepage
permalink: index.html
---

Welcome to DZS Halo's alternate site for our softwares. From here, you can find documentations for Halo Extension, Add-on API, and Add-ons. Use the sidebar on the left or top menu bar to start navigation.
{% include note.html content="Documentations are completed. This site is currently as primary site for time being." %}

Latest news:

<div class="post-list">
{% for post in site.posts limit:2 %}


<h2><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }} /
{% for tag in post.tags %}

<a href="{{ "tag_" | append: tag | append: ".html"}}">{{tag}}</a>{% unless forloop.last %}, {% endunless%}

{% endfor %}</span>
<p>{% if page.summary %} {{ page.summary | strip_html | strip_newlines | truncate: 160 }} {% else %} {{ post.content | truncatewords: 50 | strip_html }} {% endif %}</p>

{% endfor %}


{% include links.html %}
