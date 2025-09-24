---
layout: default
title: Home
---

<section class="hero">
  <h1>Hi — I’m Sreekar 👋</h1>
  <p>Trail runner • Aspiring pro • Mountain lover</p>
  <p>
    <a href="/races">Races</a> •
    <a href="/gallery">Gallery</a> •
    <a href="/blog">Blog</a> •
    <a href="/about">About</a>
  </p>
</section>

<section class="intro">
  ## Latest race
  {% assign latest = site.data.races | first %}
  {% if latest %}
  <h3>{{ latest.title }} — {{ latest.distance }} ({{ latest.elevation }})</h3>
  <p><a href="{{ latest.strava_url }}" target="_blank">View on Strava</a></p>
  {% endif %}
</section>
