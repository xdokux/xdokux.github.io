---
layout: default
title: Transmissions
---

# Transmissions

{% for post in site.posts %}
<article class="post" id="transmission-{{ forloop.index }}">
  <h2 class="post-title">
    <a href="{{ post.url }}">{{ post.title }}</a>
  </h2>

  <p class="post-date">
    {{ post.date | date: "%b %d, %Y" }}
  </p>

  <p class="post-content">
    {{ post.excerpt }}
  </p>
</article>
{% endfor %}
