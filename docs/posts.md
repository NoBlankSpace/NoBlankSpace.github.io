---
layout: default
title: Posts
permalink: /posts
---

# Posts

I write about design, technology, and research quite broadly - with the occasional miscellaneous post. I use this space to send links to people, so I hope you find something interesting. If you do - and have any comments, questions, chat intentions - please do reach out at *ben (at) searle (dot) hu*!

{% for post in site.posts %}
  <div style="padding-bottom:10px">
    <span>{{ post.date | date: "%Y.%m.%d" }}</span> <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </div>
{% endfor %}