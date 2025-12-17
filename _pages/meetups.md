---
layout: default
title: Meetups
permalink: /meetups/
---

# Meetups

We’re a Brooklyn chess hang. Bring a board if you’ve got one—if not, no stress.

## Weekly schedule

{% assign meetups = site.data.meetups %}

<div class="cards">
{% for m in meetups %}
  <div class="card">
    <div class="card-title">{{ m.name }}</div>
    <div class="card-meta">{{ m.when }} • {{ m.time }}</div>
    <div class="card-body">
      <div><strong>{{ m.location_name }}</strong></div>
      <div class="muted">{{ m.address }}</div>
      <p>{{ m.notes }}</p>
      <a class="btn" href="https://www.google.com/maps/search/?api=1&query={{ m.map_query | uri_escape }}" target="_blank" rel="noopener">Get directions</a>
    </div>
  </div>
{% endfor %}
</div>

## What to expect

- **All levels welcome.** Total beginner to absolute killer.
- **Low commitment.** Drop in, play a game, bounce.
- **Friendly chaos.** It’s social, it’s Brooklyn, it’s chess.

## Weather / cancellations

Tuesday plaza + weekend park meetups are **weather dependent**. If it’s sketchy out, we’ll call it on Instagram.

<div class="cta-row">
  <a class="btn btn-primary" href="https://www.instagram.com/prospectparkchess/" target="_blank" rel="noopener">Check updates on Instagram</a>
</div>
