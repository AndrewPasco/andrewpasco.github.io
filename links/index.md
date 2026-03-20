---
layout: single
title: Links & Articles
permalink: /links/
author_profile: true
---

A collection of articles, publications, and web links related to my work and personal accomplishments.

<div class="links-grid">
{% for item in site.data.links %}
  <a class="link-card" href="{{ item.url }}" target="_blank">
    {% if item.image %}
    <img class="link-thumb" src="{{ item.image | relative_url }}" alt="{{ item.title }}">
    {% else %}
    <div class="link-thumb"></div>
    {% endif %}

    <div class="link-content">
      <div class="link-title">{{ item.title }}</div>
      <div class="link-desc">{{ item.description }}</div>
    </div>
  </a>
{% endfor %}
</div>
