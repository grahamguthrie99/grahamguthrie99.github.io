---
layout: page
title: Quotes
section: quotes
permalink: /quote/
---

<ul>
  {% assign section_posts = site.posts | where: "section", page.section %}
  {% for post in section_posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a><br />
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>