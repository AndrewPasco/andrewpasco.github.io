---
layout: default
title: Projects
permalink: /projects/
include_custom_css: true
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
    <li><a href="#thesis">Smartphone Gesture-Based Robot Teleoperation</a></li>
    <li><a href="#consult">Student Consultancy Projects</a></li>
    <li><a href="#backgammon">Interactive Robot Backgammon</a></li>
    <li><a href="#me72">Game-Playing Mobile Robots</a></li>
    <li><a href="#lattice">Lunar Cable-Traversal Robot</a></li>
    <li><a href="#me14">Two-Stage Transmission</a></li>
  </ul>
  <h3>In Progress</h3>
  <ul>
    <li><a href="#cs229">Pose Estimation of Uncooperative Satellites</a></li>
    <li><a href="#cs230">Learning-Based Visuo-Tactile Tendon Perception</a></li>
  </ul>
</div>


<!-- Main Content -->

<h1>Projects</h1>

<p>Academic and extracurricular projects involving robotics and control, mechanical design, and machine learning.</p>

<div class="project-pane" id="thesis">
  <h2>MPhil Thesis: Exploring Smartphone-Enabled Gesture Input for Intuitive Robot Teleoperation</h2>
  <div class="project-meta">
    <span class="project-date">January 2024 – August 2025</span>
    <span class="project-location">Cambridge, UK</span>
  </div>
  <div class="project-desc">
    <img src="/assets/projects/thesis1.png">
    <p>One key challenge for robot teleoperation is broadening accessibility beyond specialized users. Many current systems rely on specialist, sometimes expensive, hardware that is not widely available to various groups of users. A promising new direction is the use of everyday devices (e.g., smartphones) as controllers to make teleoperations more affordable and accessible to a broader audience.</p>
    <p>To that end, this dissertation involved development and user testing of a hand pose and gesture-based, smartphone-enabled teleoperation system. The system combines the availability of standard consumer technology with the usability, intuitive motion mapping, and lightweight nature of vision-based teleoperation methods. Testing was completed across the Atlantic ocean, with users in the UK controlling a robot in the US.</p>
    <p>The system was developed around the iPhone 14-deployed TeleopLab. This iOS device was chosen as the development platform due to the mass-market adoption of iPhone devices and the TrueDepth camera array. Code was written in Swift 5, with MediaPipe GestureRecognizer used for hand detection and gesture classification. Three gestures enabled tethering the robot to the user’s palm pose, toggling the gripper open and closed, and resetting to a home position. The control system was built on ROS Noetic, with the host computer using the Ubuntu 20.04 OS.</p>
  </div>
</div>

<div class="project-pane" id="consult">
  <h2>MPhil Student Industrial Consultancy Projects</h2>
  <div class="project-meta">
    <span class="project-date">December 2024 – March 2025</span>
    <span class="project-location">Cambridge, UK</span>
  </div>
  <div class="project-desc">
    <p>A key part of the MPhil in Industrial Systems, Manufacture, and Management was completion of four industrial consulting projects across England and Wales involving data analysis, process optimization, and strategic recommendations. I completed three projects, each with a different partner from the cohort, during two-week stretches of in-person work with a company, speaking with operators and management and directly observing processes to generate recommendations.</p>
    <h3>RAM Innovations</h3>
    <p> The first project was an operations improvement effort at RAM Innovations, an embedded die semiconductor manufacturer in Wales. The company was interested in determining insights for low-cost potential applications of lean manufacturing principles as well as implementation a rudimentary ERP system for improved stock-keeping.</p>
    <img src="/assets/projects/ram-1.png">
    <p>By conducting interviews and assessing the production halls, we came to conclude that there are improvements needed on seven different elements of the manufacturing operations. We provided an implementation roadmap for usage by the company.</p>
    <h3>9Barista</h3>
    <p>This SME based in Cambridge possessed mature operations for production of its flagship product, the 9Barista. However, development of new products during the last three years had been slower than desired, and the speed of iteration of integrated prototypes was a particular pain point. The intention of this project was to determine how existing capabilities contribute to design iteration then identify opportunities for improvement. The approach focused on two key elements:</p>
    <ol>
      <li>Investigation of current R&D process and identification of contributors and detractors to development speed</li>
      <li>Determination of alterations and enhancements to existing process elements which can create additional speed, especially during design iteration</li>
    </ol>
    <img src="/assets/projects/9bar-1.png">
    <p>As a result of the investigation, three phases were identified as areas of potential improvement: the need for additional structure during product conceptualization and requirements definition, the need to alter project management techniques while planning for the design iteration loop, and the high resource allocation during the fabrication phase. Recommendations were identified which could help to reduce iteration cycles by 5-11 days.</p>
    <img src="/assets/projects/9bar-2.png">
    <h3>Huhtamaki BCP</h3>
    <p>Work-in-progress (WIP) management was a prevalent issue at Huhtamaki BCP. The imbalance of the production line, absence of a WIP tracking system and long dwells of WIP on the shop floor and in the storage areas had led to an elevated WIP pallet congestion problem. It was projected that Huhtamaki BCP is spending £750,000/yr to combat its WIP pallet congestion problem.</p>
    <p>The objectives for this project were process-mapping of current WIP storage/flow, identifying factors contributing to high levels of shop floor WIP, and determining WIP pallet storage based on the current situation and future requirements.</p>
    <img src="/assets/projects/bcp-1.png">
    <p>The approach adopted for this project included Gemba walks, interviews, process and value stream maps and development of solutions from root cause analysis. Solutions were produced to prevent WIP buildup, address WIP tracking and demarcation of storage, and alter the QA hold decision process.</p>
    <img src="/assets/projects/bcp-2.png">
    <p>The impact of the identified solutions was projected to produce an annual net savings of £450,000 and a 5-day improvement in average lead times.</p>
    <h3>SHS One Technologies</h3>
    <p>The fourth project was completed during the second term of coursework, so one day per week of virtual work was dedicated to this strategy development and market entry strategy project for an early-stage startup.</p>
    <img src="/assets/projects/shs-1.png">
    <p>SHS One Technologies, Ltd. (SOT) is a micro-SME planning to apply innovations in advanced hard coatings for industrial applications. Their solution offers superior materials utilization and cycle times compared to current industry standards, but they needed a formal strategy for commercialization. The agricultural and automotive sectors were identified as candidates for initial market entry. This project intended to analyse both markets, formalize a business case, and contextualise critical intellectual property considerations:</p>
    <ol>
      <li>SOT’s coating technology was analysed to define the unique value proposition and technical feasibility of SHS.</li>
      <li>A comprehensive market assessment was conducted to identify key opportunities and entry barriers in the agricultural and automotive industries, incorporating market sizing and value chain analysis.</li>
      <li>Critical insights into market dynamics were obtained by researching the industry and benchmarking the competitors, refining the evaluation of potential business models.</li>
      <li>Actionable recommendations were formulated to align with SOT’s capabilities, financial constraints and long-term growth objectives through a systematic comparison of market entry strategies.</li>
    </ol>
    <p>The key recommendations were confidential given the company’s early-stage state.</p>
  </div>
</div>

<div class="project-pane" id="backgammon">
  <h2>ME/CS/EE 134: Robotic Systems - Interactive Robot Backgammon</h2>
  <div class="project-meta">
    <span class="project-date">January 2024 – March 2024</span>
    <span class="project-location">Pasadena, CA</span>
  </div>
  <div class="project-desc">
    <img src="/assets/projects/backgammon2.png">
    <p>In Caltech's ME134 (Robotic Systems), teams of three or four develop a 5-7 degree of freedom (DOF) arm that plays a game or completes an interactive task. My team decided to tackle the challenge of making a robot that you could play backgammon against. While the majority of the challenge in this class was indeed creation of an effective software framework, sound mechanical design was also imperative to achieve millimeter-precise pointing accuracy.</p>
    <p>We determined the need for five DOFs because we wanted to manipulate objects both from a "handshaking" wrist position (for grabbing the dice cup) and a "picking" position (for grabbing the checkers and dice). Though we did not end up needing to grab the cup, we still utilized the fourth and fifth DOFs to ensure that our gripper had both the appropriate pitch position to remain parallel to the table and the appropriate yaw position to ensure we only grabbed the intended checker without conflicting against nearby checkers.</p>
    <img src="/assets/projects/backgammon1.png">
    <p>Both arm links were 450mm long and made of lasercut wood joined into a box to reduce torsional deflection. The equal link length was determined because we wanted to be able to utilize only a single work table and grab checkers on the near side of the board, very close to the base of the robot. Joint brackets were 3D printed PLA.</p>
    <p>The initial gripper was designed to grab checkers, dice, and a cup. To handle all of these, it was larger and thicker, which meant that it was more likely to bump into other checkers when attempting to grab one. Once we reduced our scope and swapped to virtual dice rolls, we accordingly modified our gripper to be more specialized for grabbing checkers.</p>
    <img src="/assets/projects/backgammon4.png">
    <p>For the software, the system consisted of three main ROS nodes. The Detector node was continuously subscribed to the raw camera feed from the top view camera and published the detected position of all checkers and the board. Checkers were detected based on their colors and features, then filtered for existence and correspondence, before finally being sorted based on their positions. The Game node handled the high level playing state of the robot during the game. It generated a set of moves encoded by [source, destination, color] by subscribing to the Detector node’s published game states. This allowed the Game node to always have a real time accurate representation of the current game state.</p>
    <img src="/assets/projects/backgammon3.png">
    <p>Finally, the Trajectory node handled the robot motion planning. It received the location of the checkers and the location of the board from the Detector node, as well as sequences of moves from the Game node. Inverse kinematics were implemented with thresholded singular value decomposition, and trajectory management was handled by queueing six specially defined TaskObjects which atomized different specific motions. There were no obstacles in the workspace, so task- or joint-space splining between waypoints was a sufficient planning method.</p>
    <img src="/assets/projects/backgammon5.png">
    <p>Beyond creation of the robot and software, we also needed to make a giant backgammon board! We lasercut the board in two halves from the same wood used for the links and laser etched features to aid our painting process. 40mm checkers were 3D printed from PLA and sanded to reduce glare.</p>
  </div>
</div>

<div class="project-pane" id="me72">
  <h2>ME72: Engineering Design Laboratory - Game-Playing Mobile Robots</h2>
  <div class="project-meta">
    <span class="project-date">September 2022 – March 2023</span>
    <span class="project-location">Pasadena, CA</span>
  </div>
  <div class="project-desc">
    <img src="/assets/projects/me72-5.jpg">
    <p>Each year, Caltech ME undergrads form teams of 3-6 to compete in ME72, a capstone engineering design competition. My year, our competition required collecting balls, shooting them into goals, and autonomously navigating an obstacle course with two mobile robots and one stationary shooter.</p>
    <p>Our team divided loosely into three sub-teams working on each robot, and I designed and built the shooter robot with a teammate. I designed the shooting tower, articulating turret, structure, and electronics, while he worked on the ball hopper, management, and agitation.</p>
    <img src="/assets/projects/me72-1.png">
    <p>Most of the shooter tower parts were made from waterjet aluminum plate, with some plate bending and other finishing ops. Right before the competition, we opted to replace the shooting curve made from wooden dowels for a 3D printed hood with a smoother profile that gave a more consistent shot. The hood was mounted to a turntable bearing and articulated with a servo-controlled linkage so it could aim at either of two adjacent goals. We used a mix of thick acrylic and thinner plastic sheeting to give the hopper semi-flexible walls.</p>
    <img src="/assets/projects/me72-2.png">
    <p>Around three weeks before the competition, our team realized that the third robot, which collected and dumped balls into the shooter, was essentially nonfunctional due to poor initial choice of gear reductions. I took on the challenge of fixing the four bar linkage by adding an additional reduction stage, choosing to waterjet these new gears instead of purchasing them and mill the new towers out of leftover stock to minimize downtime. Another teammate fixed the drivetrain, and we were testing again before the end of the week!</p>
    <img src="/assets/projects/me72-3.png">
    <p>At the final competition, our team placed second. The shooter was extremely reliable, with one wiring mishap that was fixed between rounds with the help of good documentation. My course experience motivated me to be a TA for the following year's competition, "Airship Quadball."</p>
  </div>
</div>

<div class="project-pane" id="lattice">
  <h2>LATTICE: Lunar Architecture for Tree Traversal In-service-of Cabled Exploration</h2>
  <div class="project-meta">
    <span class="project-date">September 2022 – Dec 2023</span>
    <span class="project-location">Pasadena, CA</span>
  </div>
  <div class="project-desc">
    <p>At the beginning of my junior year, I returned to campus a month early to work with Caltech Air and Outer Space on the 2022 NASA BIG Idea Challenge. The challenge concerned new methods for maneuvering on the moon, and our idea was a cable-riding shuttle. Most of the ideation was complete by the time I joined the project, so my role was in transitioning the shuttle from concept to product.</p>
    <p>I optimized component designs, combining learnings from my summers at Beta with statics knowledge and FEA methods developed through coursework. My modeling, design, and analysis verified adherence to mass and balance requirements before fabrication began.</p>
    <img src="/assets/projects/lattice-1.png">    
    <p>The shuttle utilized a self-tensioning design with articulating arms that wrap the cable around the driving pulleys to climb extreme slopes. The carbon fiber tubing used for the shuttle frame allowed it to withstand the extreme tensile forces this caused on the frame. End caps were bonded to the tubes with epoxy, allowing tubes and plates to be bolted together.</p>
    <p>Next, I fabricated the gearbox plates and passive outer pulleys for the shuttle. These aluminum plates supported the belt reduction from the motors to the driven pulleys and were designed with functionality and weight savings in mind. These were waterjet out-of-house due to time constraints, with finishing features completed on a manual mill. I also made passive pulleys for the end of the tension arms with a CNC lathe.</p>
    <img src="/assets/projects/lattice-2.jpg">
    <p>Finally, we conducted testing in the Lucerne Valley to validate performance to our intended specifications.</p>
  </div>
</div>

<div class="project-pane" id="me14">
  <h2>ME14: Design and Fabrication - Two-Stage Transmission</h2>
  <div class="project-meta">
    <span class="project-date">April 2022 – June 2022</span>
    <span class="project-location">Pasadena, CA</span>
  </div>
  <div class="project-desc">
    <p>After ME13, in which all ME students at Caltech learn how to use the mill, lathe, lasercutter, waterjet, and 3D printer, ME14 is the first class where we get to take our coursework beyond theory and engineering fundamentals into the shop. We learned fundamentals of GD&T, how to choose motors and other components for mechanical systems, and other engineering best practices (courtesy of Shigley’s).</p>
    <img src="/assets/projects/me14-1.jpg">
    <p>The main project of our ME14 was a transmission design. Given a motor powered at 12V nominal, a bike wheel load, and a required transmission footprint, we designed a two-stage geared transmission. The plates were milled from acrylic stock, and the shafts were turned from steel shaft stock. Gears were purchased off the shelf.</p>
    <img src="/assets/projects/me14-2.png">
  </div>
</div>

<p>I'm always working on something new, whether in or out of the classroom, so stay tuned for new projects!</p>

<h1>In Progress</h1>

<div class="project-pane" id="cs229">
  <h2>CS229: Machine Learning - Point Cloud Mapping for Pose Estimation of Uncooperative Satellites</h2>
  <div class="project-meta">
    <span class="project-date">September 2025 - December 2025</span>
    <span class="project-location">Stanford, CA</span>
  </div>
  <div class="project-desc">
    <p>Blurb about ongoing 229 project tbd</p>
    <img src="/assets/projects/proposed_pipeline.png">
    <p>Second blurb about model selection and implementation details</p>
    <img src="">
    <p>Third blurb with final results</p>
  </div>
</div>

<div class="project-pane" id="cs230">
  <h2>CS230: Deep Learning - Learning-Based Visuo-Tactile Tendon Perception</h2>
  <div class="project-meta">
    <span class="project-date">September 2025 - December 2025</span>
    <span class="project-location">Stanford, CA</span>
  </div>
  <div class="project-desc">
    <p>Blurb about ongoing 230 project tbd, explaining </p>
    <img src="/assets/projects/cs230-1">
    <p>Second blurb about model selection and implementation details, explain different methods for approach and intended outcomes</p>
    <img src="">
    <p>Third blurb with final results</p>
  </div>
</div>


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