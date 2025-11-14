---
layout: default
title: Projects
permalink: /projects/
---

{% include nav.html %}

# Projects

<style>
.project-pane { margin: 36px 0; padding: 12px 0; border-bottom: 1px solid #e6e6e6; }
.project-pane h2 { margin: 12px 0; }
.project-desc { max-width: 900px; margin: 12px auto; font-size: 16px; }
</style>

<div class="project-pane">
  <h2>Interactive Robot Backgammon</h2>

  {% include carousel.html
     id="carousel-backgammon"
     images="/assets/projects/backgammon1.png,/assets/projects/backgammon2.png,/assets/projects/backgammon3.png"
  %}

  <div class="project-desc">
    <p>Built a ROS2-controlled tabletop backgammon robot with motion planning,
    OpenCV vision pipelines, and integrated game logic. Demonstrated 20 minutes
    of fully autonomous, error-free gameplay.</p>
  </div>
</div>

<!-- <div class="project-pane">
  <h2>Gesture-Based Smartphone Robot Teleoperation</h2>

  {% include carousel.html
     id="carousel-teleop"
     images=["/assets/projects/teleop1.jpg","/assets/projects/teleop2.jpg"]
  %}

  <div class="project-desc">
    <p>Developed a smartphone hand-pose & gesture teleoperation interface.
    Integrated with ROS1, performed user studies, and submitted a first-author
    ICRA 2026 manuscript in collaboration with MIT LEAP.</p>
  </div>
</div> -->

<div class="project-pane">
  <h2>ME72 - Engineering Design Laboratory</h2>

  {% include carousel.html
     id="carousel-me72"
     images="/assets/projects/me72-1.png,/assets/projects/me72-22.png,/assets/projects/me72-3.png,/assets/projects/me72-4.png"
  %}

  <div class="project-desc">
    <p>Each year, Caltech ME undergrads form teams of 3-6 to compete in ME72, a capstone engineering design competition. My year, our competition required collecting balls, shooting them into goals, and autonomously navigating an obstacle course with two mobile robots and one stationary shooter.
    Our team divided loosely into three sub-teams working on each robot, and I designed and built the shooter robot with a teammate. I designed the shooting tower, articulating turret, structure, and electronics, while he worked on the ball hopper, management, and agitation.
    Most of the shooter tower parts were made from waterjet aluminum plate, with some plate bending and other finishing ops. Right before the competition, we opted to replace the shooting curve made from wooden dowels for a 3D printed hood with a smoother profile that gave a more consistent shot. The hood was mounted to a turntable bearing and articulated with a servo-controlled linkage so it could aim at either of two adjacent goals. We used a mix of thick acrylic and thinner plastic sheeting to give the hopper semi-flexible walls.
    .</p>
  </div>
</div>
