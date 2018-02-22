---
layout: home
title: Home
landing-title: 'Hi, this is Open Source Africa'
author: OscAfrica
---
  {% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.image }} 
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}