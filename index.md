---
layout: default
title: Prospect Park Chess Club
permalink: /
header_type: hero
header_img: /assets/img/hero/hasenstuble.png
---

<div class="hero">
  <div class="hero-inner">
    <div class="eyebrow">Brooklyn chess • all levels</div>
    <h1>Prospect Park Chess Club</h1>
    <p class="lead">A friendly, slightly rowdy chess hang in Brooklyn. Drop in, play a game, meet people.</p>

    <div class="cta-row">
      <a class="btn btn-primary" href="{{ '/meetups/' | relative_url }}">See meetup schedule</a>
      <a class="btn btn-ppcc2" href="{{ '/about/' | relative_url }}">About</a>
      <a class="btn btn-ppcc2" href="{{ '/faq/' | relative_url }}">FAQ</a>
    </div>
    <div class="cta-row">
      <a class="btn btn-ppcc" href="{{ '/newb/' | relative_url }}">If its your first time CLICK HERE</a>
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
          <a class="btn btn-ppcc3" href="https://www.google.com/maps/search/?api=1&query={{ m.map_query | uri_escape }}" target="_blank" rel="noopener">Get directions</a>
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
    <li>Bringing boards/clocks is not required. We have everything you need.</li>
    <li>There's a drink special at the bar. Ask for a "Chess Beer."</li>
  </ul>
</section>
