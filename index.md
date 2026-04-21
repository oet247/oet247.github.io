---
layout: default
title: Home
---

Hello and welcome to Right some of the times, my blog about YOMI hustle, anime and a lot of other things.

The site is still relatively bare bones and will continue to remain so until I get enough time to make it look nice. For now, this is all I have to work with.

Heres a link to my [superdoc] (https://docs.google.com/document/d/1wscCT6eiMVhm0hXO4OV_gyRr2LvytKG-9OvlJjTPIc8/edit?tab=t.0), which I will eventually transfer all of into here (by eventually, I mean in the next 24, and then this section will be entirely redundant)

---

## Posts

{% for post in site.posts %}
  <h2>
    <a href="{{ post.url | relative_url }}">
      {{ post.title }}
    </a>
  </h2>
  <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
  <p>{{ post.date | date: "%b %d, %Y" }}</p>
  <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>

  <hr>
{% endfor %}

