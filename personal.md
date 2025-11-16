---
layout: default
title: Personal
permalink: /personal/
---

{% include nav.html %}

{% include sidebar.html %}

<!-- Fixed Sidebar -->
<div class="sidebar">
  <h3>Personal</h3>
  <ul>
    <li><a href="#athletics">Athletics</a></li>
    <li><a href="#travel">Travel</a></li>
    <li><a href="#other">Other Interests</a></li>
  </ul>
</div>

<!-- Main Content -->

<h1>Personal</h1>

<div class="section-pane" id="athletics">
  <h2>Athletics</h2>
  <p>I’ve always balanced academics with athletics: swimming, strength training, and now long-distance endurance events.</p>
  <p>Before the end of undergrad, swimming was my most important commitment outside of my academics. A few highlights include:</p>
  <ul>
    <li>Helping Caltech place 3rd at SCIAC Championships in 2022 and 2023, tying our highest-ever finish</li>
    <li>Setting school records in the 200 I.M. (1:51.92) and 400 I.M. (4:01.11) at the 2024 SCIAC Championships</li>
    <li>Receiving the SCIAC Character Award and Caltech Director's award at the end of my final year</li>
  </ul>
  <div class="personal-gallery">
    <img src="{{ '/assets/personal/swim-1.jpg' | relative_url }}" alt="swim pic 1">
    <img src="{{ '/assets/personal/swim-2.jpg' | relative_url }}" alt="swim pic 2">
    <img src="{{ '/assets/personal/swim-6.jpg' | relative_url }}" alt="swim pic 3">
    <img src="{{ '/assets/personal/swim-3.jpg' | relative_url }}" alt="swim pic 4">
    <img src="{{ '/assets/personal/swim-5.jpg' | relative_url }}" alt="swim pic 5">
    <img src="{{ '/assets/personal/swim-4.jpg' | relative_url }}" alt="swim pic 6">
  </div>
  <p>I'm currently training for an **Ironman 70.3** (Oceanside 2026), which has been a fun long-term training goal in my post-swimming life.</p>
  <p>Between the end of swimming at Caltech and this new goal, I have raced in a few 5ks, a 10k, and the Cambridge Half Marathon.</p>
  <div class="personal-gallery">
    <img src="{{ '/assets/personal/cam-half.jpg' | relative_url }}" alt="cam half marathon">
    <img src="{{ '/assets/personal/bike.jpg' | relative_url }}" alt="bike photo">
  </div>
  <p>I also competed with the Cambridge Blues Swimming Team and the Water Polo Seconds Team in the 2025 varsity matches against Oxford!</p>
  <div class="personal-gallery">
    <img src="{{ '/assets/personal/cam-swim.jpg' | relative_url }}" alt="Cam Swim Varsity">
    <img src="{{ '/assets/personal/wapo.jpg' | relative_url }}" alt="Cam WP Varsity">
  </div>
</div>

<div class="section-pane" id="travel">
<h2>Travel</h2>
  <p>I love exploring new cities, cultures, and experiencing other regions' nature.</p>
  <p>Here are a few memorable stops:</p>
  <ul>
    <li>Spending two weeks in Vietnam (visiting Ho Chi Minh City and the surrounding area) and Cambodia (visiting the Angkor Archaeological Park)</li>
    <li>Hiking in national parks across the US, including Zion, Bryce Canyon, and Grand Teton</li>
    <li>Visiting Seoul, Tokyo, and Jeju Island</li>
    <li>Seeing industrial sites and locations of cultural importance across France, including Bordeaux, Lyon, Paris, and Lille</li>
  </ul>
  <div class="personal-gallery">
    <img src="{{ '/assets/personal/angkor.jpg' | relative_url }}" alt="Ta Prohm">
    <img src="{{ '/assets/personal/jackson.jpg' | relative_url }}" alt="frozen jackson lake">
    <img src="{{ '/assets/personal/korea.jpg' | relative_url }}" alt="Seoul">
    <img src="{{ '/assets/personal/eiffel.jpg' | relative_url }}" alt="Eiffel Tower">
  </div>
</div>

<div class="section-pane" id="other">
  <h2>Other Interests</h2>
  <p>My other interests include hiking, music (particularly listening to analyses of popular narrative albums and expanding my tastes!), flying, and cooking.</p>
  <div class="personal-gallery">
    <img src="{{ '/assets/personal/hike.jpg' | relative_url }}" alt="other interests photo 1">
    <img src="{{ '/assets/personal/extra.jpg' | relative_url }}" alt="other interests photo 2">
  </div>
</div>

<!-- Style Specifics -->

<style>
.personal-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
  gap: 18px;
  margin-top: 16px;
}
.personal-gallery img {
  width: 100%;
  height: 300px;
  border-radius: 12px;
  object-fit: cover;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}
</style>