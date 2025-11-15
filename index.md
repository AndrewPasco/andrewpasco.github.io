---
layout: default
title: Home
---

# Welcome

<div class="home-grid">
  <a href="/projects/" class="grid-item">
    <img src="/assets/projects/backgammon1.png" alt="Projects">
    <div class="grid-label">Projects</div>
  </a>
  
  <a href="/resume/" class="grid-item">
    <img src="/assets/misc/gradcap.png" alt="Resume">
    <div class="grid-label">Resume</div>
  </a>

  <a href="/links/" class="grid-item">
    <img src="/assets/links/pasco-schilt-thumb.jpg" alt="Links">
    <div class="grid-label">Links</div>
  </a>

  <a href="/personal/" class="grid-item">
    <img src="/assets/personal/jackson.jpg" alt="Personal">
    <div class="grid-label">Personal</div>
  </a>
</div>

<style>
/* 2x2 grid */
.home-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 24px;
  max-width: 900px;
  margin: 24px auto;
}

/* Each thumbnail card */
.grid-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  text-decoration: none;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 16px;
  background: #f8f8f8;
  transition: transform 0.2s, box-shadow 0.2s;
}

.grid-item:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 16px rgba(0,0,0,0.15);
}

.grid-item img {
  width: 120px;
  height: 120px;
  object-fit: cover;
  border-radius: 6px;
  margin-bottom: 12px;
}

.grid-label {
  font-size: 18px;
  font-weight: 600;
  color: #333;
}
</style>
