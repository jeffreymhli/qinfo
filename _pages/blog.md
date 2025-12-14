---
layout: page
permalink: /blog/
title: Blog
description: Some of my little findings and learning repositories.
nav: true
nav_order: 2
---

<div class="post-list">
  {% for post in site.posts %}
    <div class="post-preview" style="margin-bottom: 30px;">
      <h3>
        <a href="{{ post.url | relative_url }}" style="color: #0056b3; text-decoration: none;">
          {{ post.title }}
        </a>
      </h3>
      <p style="color: #666; font-size: 0.9rem;">
        {{ post.date | date: "%B %-d, %Y" }}
      </p>
      <p>
        {{ post.description }}
      </p>
    </div>
  {% endfor %}
</div>