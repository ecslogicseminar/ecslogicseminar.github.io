---
layout: default
title: Home
---
# Logic Seminars
Here you can find all logic seminars, and a schedule for future ones [here](https://sotonac-my.sharepoint.com/:x:/g/personal/jmmg1c24_soton_ac_uk/EYfw8Tg9DdtNsHLqqdiy47UBLqt4fazyoDzmxdcjvN1TuQ?e=UN0lgY).
## Upcoming Seminars & Events

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
