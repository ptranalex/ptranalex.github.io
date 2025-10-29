---
layout: home
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/header-bg.jpg
  actions:
    - label: "Explore My Projects"
      url: "/portfolio/"
    - label: "Read My Writing"
      url: "/blog/"
excerpt: "Exploring the intersection of engineering, AI, and meaningful products — one experiment at a time."
feature_row:
  - image_path: /assets/images/portfolio-thumb.jpg
    alt: "Portfolio"
    title: "Projects"
    excerpt: "A collection of things I’ve built — from AI agents and automation tools to production-scale web systems."
    url: "/portfolio/"
    btn_label: "View Projects"
    btn_class: "btn--primary"
  - image_path: /assets/images/blog-thumb.jpg
    alt: "Blog"
    title: "Writing"
    excerpt: "Reflections on technology, leadership, and the craft of building with purpose."
    url: "/blog/"
    btn_label: "Read Posts"
    btn_class: "btn--primary"
  - image_path: /assets/images/about-thumb.jpg
    alt: "About"
    title: "About Me"
    excerpt: "Developer, product thinker, and lifelong learner — currently building systems that blend code and creativity."
    url: "/about/"
    btn_label: "Learn More"
    btn_class: "btn--primary"
---

{% include feature_row %}

## Recent Posts

<div class="grid__wrapper">
  {% for post in site.posts limit:3 %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
