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

  <h2>{{ year.name }}</h2>
  {% for post in year.items %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
