---
layout: default
title: Projects
permalink: /projects/
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
    <li><a href="#thesis">MPhil Thesis</a></li>
    <li><a href="#consult">MPhil Industrial Consultancy Projects</a></li>
    <li><a href="#backgammon">Interactive Robot Backgammon</a></li>
    <li><a href="#me72">ME72 – Engineering Design Laboratory</a></li>
  </ul>
</div>


<!-- Main Content -->
<div class="project-content">
  # Projects

  <div class="project-pane" id="thesis">
    <h2>MPhil Thesis: Exploring Smartphone-Enabled Gesture Input for Intuitive Robot Teleoperation</h2>

    {% include carousel.html
      id="carousel-backgammon"
      images="/assets/projects/thesis1.png,/assets/projects/thesis2.png,/assets/projects/thesis3.png"
    %}

    <div class="project-desc">
      <p>One key challenge for robot teleoperation is broadening accessibility beyond specialized users. Many current systems rely on specialist, sometimes expensive, hardware that is not widely available to various groups of users. A promising new direction is the use of everyday devices (e.g., smartphones) as controllers to make teleoperations more affordable and accessible to a broader audience.</p>
      <p>To that end, this dissertation involved development and user testing of a hand pose and gesture-based, smartphone-enabled teleoperation system. The system combines the availability of standard consumer technology with the usability, intuitive motion mapping, and lightweight nature of vision-based teleoperation methods. Testing was completed across the Atlantic ocean, with users in the UK controlling a robot in the US.</p>
      <p>The system was developed around the iPhone 14-deployed TeleopLab. This iOS device was chosen as the development platform due to the mass-market adoption of iPhone devices and the TrueDepth camera array. Code was written in Swift 5, with MediaPipe GestureRecognizer used for hand detection and gesture classification. Three gestures enabled tethering the robot to the user’s palm pose, toggling the gripper open and closed, and resetting to a home position. The control system was built on ROS Noetic, with the host computer using the Ubuntu 20.04 OS.</p>
    </div>
  </div>

  <div class="project-pane" id="consult">
    <h2>MPhil Student Industrial Consultancy Projects</h2>

    {% include carousel.html
      id="carousel-backgammon"
      images="/assets/projects/9barista.png,/assets/projects/SHS1.png,/assets/projects/bcp.png"
    %}

    <div class="project-desc">
      <p>A key part of the MPhil in Industrial Systems, Manufacture, and Management was completion of four industrial consulting projects across England and Wales involving data analysis, process optimization, and strategic recommendations. I completed three projects, each with a different partner from the cohort, during two-week stretches of in-person work with a company, speaking with operators and management and directly observing processes to generate recommendations.</p>
      <p> The first project was an operations improvement effort at RAM Innovations, an embedded die semiconductor manufacturer in Wales. The company was interested in determining insights for low-cost potential applications of lean manufacturing principles as well as implementation a rudimentary ERP system for improved stock-keeping.</p>
      <img src="/assets/projects/ram-1.png">
      <p>By conducting interviews and assessing the production halls, we came to conclude that there are improvements needed on seven different elements of the manufacturing operations. We provided an implementation roadmap for usage by the company.</p>
      <p>The fourth project was completed during the second term of coursework, so one day per week of virtual work was dedicated to this strategy development and market entry strategy project for an early-stage startup</p>
    </div>
  </div>

  <div class="project-pane" id="backgammon">
    <h2>Interactive Robot Backgammon</h2>

    {% include carousel.html
      id="carousel-backgammon"
      images="/assets/projects/backgammon1.png,/assets/projects/backgammon2.png,/assets/projects/backgammon3.png"
    %}

    <div class="project-desc">
      <p>In Caltech's ME134 (Robotic Systems), teams of three or four develop a 5-7 degree of freedom (DOF) arm that plays a game or completes an interactive task. My team decided to tackle the challenge of making a robot that you could play backgammon against. While the majority of the challenge in this class was indeed creation of an effective software framework, sound mechanical design was also imperative to achieve millimeter-precise pointing accuracy.</p>
      <p>We determined the need for five DOFs because we wanted to manipulate objects both from a "handshaking" wrist position (for grabbing the dice cup) and a "picking" position (for grabbing the checkers and dice). Though we did not end up needing to grab the cup, we still utilized the fourth and fifth DOFs to ensure that our gripper had both the appropriate pitch position to remain parallel to the table and the appropriate yaw position to ensure we only grabbed the intended checker without conflicting against nearby checkers.</p>
      <p>Both arm links were 450mm long and made of lasercut wood joined into a box to reduce torsional deflection. The equal link length was determined because we wanted to be able to utilize only a single work table and grab checkers on the near side of the board, very close to the base of the robot. Joint brackets were 3D printed PLA.</p>
      <p>The initial gripper was designed to grab checkers, dice, and a cup. To handle all of these, it was larger and thicker, which meant that it was more likely to bump into other checkers when attempting to grab one. Once we reduced our scope and swapped to virtual dice rolls, we accordingly modified our gripper to be more specialized for grabbing checkers.</p>
      <p>Beyond creation of the robot itself, we also needed to make a giant backgammon board! We lasercut the board in two halves from the same wood used for the links and laser etched features to aid our painting process. 40mm checkers were 3D printed from PLA and sanded to reduce glare.</p>
    </div>
  </div>

  <div class="project-pane" id="me72">
    <h2>ME72 - Engineering Design Laboratory</h2>

    {% include carousel.html
      id="carousel-me72"
      images="/assets/projects/me72-1.png,/assets/projects/me72-2.png,/assets/projects/me72-3.png,/assets/projects/me72-4.png"
    %}

    <div class="project-desc">
      <p>Each year, Caltech ME undergrads form teams of 3-6 to compete in ME72, a capstone engineering design competition. My year, our competition required collecting balls, shooting them into goals, and autonomously navigating an obstacle course with two mobile robots and one stationary shooter.</p>
      <p>Our team divided loosely into three sub-teams working on each robot, and I designed and built the shooter robot with a teammate. I designed the shooting tower, articulating turret, structure, and electronics, while he worked on the ball hopper, management, and agitation.</p>
      <p>Most of the shooter tower parts were made from waterjet aluminum plate, with some plate bending and other finishing ops. Right before the competition, we opted to replace the shooting curve made from wooden dowels for a 3D printed hood with a smoother profile that gave a more consistent shot. The hood was mounted to a turntable bearing and articulated with a servo-controlled linkage so it could aim at either of two adjacent goals. We used a mix of thick acrylic and thinner plastic sheeting to give the hopper semi-flexible walls.</p>
    </div>
  </div>
</div>

<!-- Styles -->
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

/* Main content pushed to right of sidebar */

/* Project panes */
.project-pane { 
  margin: 36px 0; 
  padding: 12px 0; 
  border-bottom: 1px solid #e6e6e6; 
}
.project-pane h2 { 
  margin: 12px 0; 
}
.project-desc { 
  margin: 12px 0; 
  font-size: 16px; 
}
.project-desc img {
  max-width: 100%;
  height: auto;
  margin: 12px 0;
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