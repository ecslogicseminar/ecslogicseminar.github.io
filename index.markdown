---
layout: default
title: Home
---

# Upcoming Seminars & Events

{% for post in site.posts %}
  <h2>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h2>
  <p>
    <strong>Date:</strong> {{ post.date | date: "%A, %B %-d, %Y" }} <br>
    <strong>Time:</strong> {{ post.time }} <br>
    <strong>Location:</strong> {{ post.location }} <br>
    <strong>Speaker:</strong> {{ post.speaker }}
  </p>
  <hr>
{% endfor %}
