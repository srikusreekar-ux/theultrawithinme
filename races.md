---
layout: default
title: Races
---

# Race Portfolio

<div class="race-grid">
{% for race in site.data.races %}
  <article class="race-card">
    <img src="{{ race.image }}" alt="{{ race.title }}" />
    <h2>{{ race.title }}</h2>
    <p><strong>Distance:</strong> {{ race.distance }} &nbsp; | &nbsp; <strong>Elevation:</strong> {{ race.elevation }}</p>
    <p><strong>Date:</strong> {{ race.date }} &nbsp; • &nbsp; <strong>Time:</strong> {{ race.time }}</p>
    {% if race.strava_url %}
      <p><a href="{{ race.strava_url }}" target="_blank">View on Strava</a></p>
    {% endif %}
  </article>
{% endfor %}
</div>
