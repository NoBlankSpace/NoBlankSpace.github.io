---
layout: default
---

# Posts

I write about design, technology, and research quite broadly - with the occasional miscellaneous post. I use this space to send links to people, so I hope you find something interesting. If you do - and have any comments, questions, chat intentions - please do reach out at *ben (at) searle (dot) hu*!

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}