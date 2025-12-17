---
layout: default
title: Prospect Park Chess Club
permalink: /
---

<div class="hero">
  <div class="hero-inner">
    <div class="eyebrow">Brooklyn chess • all levels</div>
    <h1>Prospect Park Chess Club</h1>
    <p class="lead">A friendly, slightly rowdy chess hang in Brooklyn. Drop in, play a game, meet people.</p>

    <div class="cta-row">
      <a class="btn btn-primary" href="/meetups/">See meetup schedule</a>
      <a class="btn" href="https://www.instagram.com/prospectparkchess/" target="_blank" rel="noopener">Instagram updates</a>
      <a class="btn" href="/merch/">Merch</a>
    </div>
  </div>
</div>

<section>
  <h2>Next up</h2>
  <p class="muted">Our schedule changes with the weather—Instagram is always current.</p>

  {% assign meetups = site.data.meetups %}
  <div class="cards">
    {% for m in meetups limit:2 %}
      <div class="card">
        <div class="card-title">{{ m.name }}</div>
        <div class="card-meta">{{ m.when }} • {{ m.time }}</div>
        <div class="card-body">
          <div><strong>{{ m.location_name }}</strong></div>
          <div class="muted">{{ m.address }}</div>
          <a class="btn" href="https://www.google.com/maps/search/?api=1&query={{ m.map_query | uri_escape }}" target="_blank" rel="noopener">Get directions</a>
        </div>
      </div>
    {% endfor %}
  </div>
</section>

<section>
  <h2>New here?</h2>
  <ul>
    <li>No membership, no signup. Just show up.</li>
    <li>Beginners welcome — we’ll get you a game.</li>
    <li>Bringing boards/clocks is appreciated but not required.</li>
  </ul>
</section>
