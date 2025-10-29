---
title: "Blog"
layout: archive
permalink: /blog/
author_profile: true
---

Welcome to my writing corner — a collection of notes, essays, and reflections from the journey of building software and teams.

Here I share thoughts on **engineering**, **AI-driven development**, and the craft of creating systems that balance performance, simplicity, and human intent.

---

{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}

  <h2 class="archive__year">{{ year.name }}</h2>
  {% for post in year.items %}
  <article class="archive__item">
    <h3 class="archive__item-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h3>
    <p class="archive__item-meta">
      <i class="far fa-calendar"></i> {{ post.date | date: "%B %d, %Y" }}
      &nbsp;·&nbsp;
      <i class="far fa-clock"></i> {{ post.read_time }} min read
    </p>
    <p class="archive__item-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
  </article>
  {% endfor %}
{% endfor %}
