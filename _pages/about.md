---
permalink: /
title: "Home Page"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
>*"The pleasure of finding things out."* — Richard Feynman

Welcome.
{% comment %}
This is a personal patch of low temperature but **high configurational entropy** — seemingly stable, but wildly fluctuating in thought-space.
{% endcomment %}

I’m an undergrad wandering (somewhat aimlessly) through a tangle of ideas in — physics, biology, algorithms — without staying long enough to unpack my bags. I like to occasionally dabble into anything else that looks like it might someday self-organize into meaning. This site is a semi-structured attempt at collecting these trails. 

------

<h2>📝 Recent Blog Posts</h2>
<ul>
  {% assign posts = site.posts | slice: 0, 3 %}
  {% for post in posts %}
    <li>
      <strong>{{ post.date | date: "%b %d, %Y" }}</strong>:
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


<!---
<h2>📚 Recent Publications</h2>
<ul>
  {% assign publications = site.publications | sort: "date" | reverse | slice: 0, 3 %}
  {% for item in publications %}
    <li>
      <strong>{{ item.date | date: "%Y" }}</strong>: 
      <a href="{{ item.url }}">{{ item.title }}</a>
    </li>
  {% endfor %}
</ul>
--->

<h2>📢 Latest Updates</h2>
<ul>
  {% assign updates = site.news | sort: "date" | reverse | slice: 0, 3 %}
  {% for update in updates %}
    <li>
      <strong>{{ update.date | date: "%b %d, %Y" }}</strong>: 
      <a href="{{ update.url }}">{{ update.title }}</a>
    </li>
  {% endfor %}
</ul>
Check out the [News Archive](/news/) for all past updates!

