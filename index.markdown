---
layout: default
title: Home
---

# Logic Seminars
Here you can find all logic seminars, and a schedule for future ones [here](https://sotonac-my.sharepoint.com/:x:/g/personal/jmmg1c24_soton_ac_uk/EYfw8Tg9DdtNsHLqqdiy47UBLqt4fazyoDzmxdcjvN1TuQ?e=UN0lgY).

## Upcoming Seminars & Events
{% assign future_events = site.posts | where_exp: "post", "post.date > site.time" | sort: "date" %}
{% if future_events.size > 0 %}
  {% for post in future_events %}
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>
    <strong>Date:</strong> {{ post.date | date: "%A, %B %-d, %Y" }} <br>
    <strong>Time:</strong> {{ post.time }} <br>
    <strong>Location:</strong> {{ post.location }} <br>
    <strong>Speaker:</strong> {{ post.speaker }}
  </p>
  <hr>
  {% endfor %}
{% else %}
  <p>No upcoming events.</p>
{% endif %}

## Past Seminars & Events
{% assign past_events = site.posts | where_exp: "post", "post.date <= site.time" | sort: "date" | reverse %}
{% if past_events.size > 0 %}
  {% for post in past_events %}
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>
    <strong>Date:</strong> {{ post.date | date: "%A, %B %-d, %Y" }} <br>
    <strong>Time:</strong> {{ post.time }} <br>
    <strong>Location:</strong> {{ post.location }} <br>
    <strong>Speaker:</strong> {{ post.speaker }}
  </p>
  <hr>
  {% endfor %}
{% else %}
  <p>No past events yet.</p>
{% endif %}
