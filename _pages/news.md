---
title: ""
layout: archive
permalink: /news/
collection: news
author_profile: false
---

<h1>📢 News Archive</h1>

<ul>
  {% assign updates = site.news | sort: "date" | reverse %}
  {% for update in updates %}
    <li>
      <strong>{{ update.date | date: "%b %d, %Y" }}</strong>: 
      <a href="{{ update.url }}">{{ update.title }}</a>
    </li>
  {% endfor %}
</ul>
