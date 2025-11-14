---
layout: default
title: Personal
permalink: /personal/
---

{% include nav.html %}

<!-- Scroll Progress Bar -->
<div id="scrollProgressContainer">
  <div id="scrollProgressBar"></div>
</div>

<!-- Fixed Sidebar -->
<div class="project-sidebar">
  <h3>Projects</h3>
  <ul>
    <li><a href="#athletics">Athletics</a></li>
    <li><a href="#travel">Travel</a></li>
    <li><a href="#other">Other Interests</a></li>
  </ul>
</div>

# Personal

---

# Athletics

I’ve always balanced academics with athletics: swimming, strength training, and now long-distance endurance events.  

Before the end of undergrad, swimming was my most important commitment outside of my academics. A few highlights include:

- Helping Caltech place 3rd at SCIAC Championships in 2022 and 2023, tying our highest-ever finish
- Setting school records in the 200 I.M. (1:51.92) and 400 I.M. (4:01.11) at the 2024 SCIAC Championships
- Receiving the SCIAC Character Award and Caltech Director's award at the end of my final year

<div class="personal-gallery">
  <img src="{{ '/assets/personal/swim-1.jpg' | relative_url }}" alt="swim pic 1">
  <img src="{{ '/assets/personal/swim-2.jpg' | relative_url }}" alt="swim pic 2">
  <img src="{{ '/assets/personal/swim-6.jpg' | relative_url }}" alt="swim pic 3">
  <img src="{{ '/assets/personal/swim-3.jpg' | relative_url }}" alt="swim pic 4">
  <img src="{{ '/assets/personal/swim-5.jpg' | relative_url }}" alt="swim pic 5">
  <img src="{{ '/assets/personal/swim-4.jpg' | relative_url }}" alt="swim pic 6">
</div>

I'm currently training for an **Ironman 70.3** (Oceanside 2026), which has been a fun long-term training goal in my post-swimming life.  

Between the end of swimming at Caltech and this new goal, I have raced in a few 5ks, a 10k, and the Cambridge Half Marathon.

<div class="personal-gallery">
  <img src="{{ '/assets/personal/cam-half.jpg' | relative_url }}" alt="cam half marathon">
  <img src="{{ '/assets/personal/bike.jpg' | relative_url }}" alt="bike photo">
</div>

I also competed with the Cambridge Blues Swimming Team and the Water Polo Seconds Team in the 2025 varsity matches against Oxford!

<div class="personal-gallery">
  <img src="{{ '/assets/personal/cam-swim.jpg' | relative_url }}" alt="Cam Swim Varsity">
  <img src="{{ '/assets/personal/wapo.jpg' | relative_url }}" alt="Cam WP Varsity">
</div>

---

# Travel

I love exploring new cities, cultures, and experiencing other regions' nature.  
Here are a few memorable stops:

- Spending two weeks in Vietnam (visiting Ho Chi Minh City and the surrounding area) and Cambodia (visiting the Angkor Archaeological Park)  
- Hiking in national parks across the US, including Zion, Bryce Canyon, and Grand Teton  
- Visiting Seoul, Tokyo, and Jeju Island  
- Seeing industrial sites and locations of cultural importance across France, including Bordeaux, Lyon, Paris, and Lille  

<div class="personal-gallery">
  <img src="{{ '/assets/personal/angkor.jpg' | relative_url }}" alt="Ta Prohm">
  <img src="{{ '/assets/personal/jackson.jpg' | relative_url }}" alt="frozen jackson lake">
  <img src="{{ '/assets/personal/korea.jpg' | relative_url }}" alt="Seoul">
  <img src="{{ '/assets/personal/eiffel.jpg' | relative_url }}" alt="Eiffel Tower">
</div>

---

# Other Interests

My other interests include:
  
- Hiking  
- Music  
- Flying
- Cooking  

<div class="personal-gallery">
  <img src="{{ '/assets/personal/hike.jpg' | relative_url }}" alt="other interests photo 1">
  <img src="{{ '/assets/personal/extra.jpg' | relative_url }}" alt="other interests photo 2">
</div>

<!-- Style Specifics -->

<style>
/* Smooth scrolling */
html { scroll-behavior: smooth; }

/* Scroll progress bar */
#scrollProgressContainer {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background: #eee;
  z-index: 9999;
}
#scrollProgressBar {
  width: 0%;
  height: 100%;
  background: #0066cc;
}

/* Sidebar */
.project-sidebar {
  position: fixed;
  top: 100px;
  left: 20px;
  width: 220px;
  padding: 16px;
  background: #f8f8f8;
  border: 1px solid #ddd;
  border-radius: 6px;
  z-index: 1000;
}
.project-sidebar h3 {
  margin-top: 0;
}
.project-sidebar ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
.project-sidebar li {
  margin: 8px 0;
}
.project-sidebar a {
  text-decoration: none;
  color: #0066cc;
}
.project-sidebar a:hover {
  text-decoration: underline;
}
.project-sidebar a.active {
  font-weight: bold;
  color: #ff6600;
}

.personal-section {
  margin: 40px 0;
}
.personal-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
  gap: 18px;
  margin-top: 16px;
}
.personal-gallery img {
  width: 100%;
  border-radius: 12px;
  object-fit: cover;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}
</style>

<!-- Scripts -->
<script>
// Scroll progress bar
window.addEventListener('scroll', function() {
  const scrollTop = window.scrollY;
  const docHeight = document.body.scrollHeight - window.innerHeight;
  const scrollPercent = (scrollTop / docHeight) * 100;
  document.getElementById('scrollProgressBar').style.width = scrollPercent + '%';
});

// Highlight current project in sidebar
const sections = document.querySelectorAll('.project-pane');
const sidebarLinks = document.querySelectorAll('.project-sidebar a');

window.addEventListener('scroll', () => {
  let current = '';
  sections.forEach(section => {
    const sectionTop = section.offsetTop - 120; // offset for nav & margin
    if (window.scrollY >= sectionTop) {
      current = section.getAttribute('id');
    }
  });

  sidebarLinks.forEach(link => {
    link.classList.remove('active');
    if (link.getAttribute('href') === '#' + current) {
      link.classList.add('active');
    }
  });
});
</script>