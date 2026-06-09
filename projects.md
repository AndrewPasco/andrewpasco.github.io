---
layout: single
title: Projects
permalink: /projects/
author_profile: true
toc: true
toc_label: "My Projects"
toc_icon: "cog"
---

Academic and extracurricular projects involving robotics and control, mechanical design, and machine learning.

# Stanford University (MS Projects)

<details open markdown="1">
<summary><span class="on-close">Click to view Stanford projects</span><span class="on-open">Collapse Stanford projects</span></summary>

## ME327: Vibrotactile Haptic Belt for Covert Communication of UAS Threat Direction {#me327}

**May 2026** | *Stanford, CA*

This project developed a wearable, eyes-free haptic interface (the "Vibro-TACTical Belt") to convey unmanned aerial system (UAS) threat directions to dismounted operators. By mapping detected drone azimuths to an array of eight eccentric rotating mass (ERM) vibration motors distributed around the user's waist at 45° intervals, the system provides immediate, body-referenced cues that do not overload visual or auditory channels. A central Particle Argon controller processes real-time global coordinate data received over Bluetooth Low Energy (BLE) from a Pygame host simulation. By fusing this data with 100Hz orientation data from an onboard BNO085 IMU, the belt translates global threat bearings into relative, body-centric haptic alerts.

To allow users to distinguish between multiple threats concurrently, the firmware features customizable haptic signatures (distinct temporal on/off vibration patterns) for up to 10 unique threat IDs, scaling the PWM intensity based on threat proximity. The mechanical architecture consists of seven custom 3D-printed modular housings (printed in black PLA) that slide and snap onto an adjustable work-belt. This modular design accommodates different waist sizes while maintaining precise motor spacing and consistent, conforming skin contact. The system was successfully demonstrated at the Stanford Haptics Open House, earning high rankings for usability, noticeability, and intuitive feedback.

**Contributions:** I developed the system's C++ firmware architecture, implementing the control loop that integrates BNO085 IMU data and BLE threat tracking logic. I also designed and fabricated the custom 3D-printed modular enclosures (blank, driver, and controller modules) to ensure a secure fit, clean wire management, and a low-profile, covert aesthetic.

![ME327 Haptic Belt](/assets/projects/me327-belt.jpg)

## ME326: Collaborative Robotics - Speech Enabled Autonomous Liquid-handler (S.E.A.L. Team 6) {#me326}

**January 2026 – March 2026** | *Stanford, CA*

This project developed **S.E.A.L. Team 6** (Speech Enabled Autonomous Liquid-handler), a voice-commanded mobile robot that responds to natural language commands to find, retrieve, and manipulate objects in cluttered environments. Built on the bimanual **TidyBot++** mobile manipulator platform, the robot integrates voice control with a visual pipeline utilizing YOLO-based detection and Gemini for reasoning. For retrieval and sorting tasks, a visual-servo state machine guides the robot to approach the target object, retrieve it, or deposit it precisely in a bowl. As a custom group challenge, the robot was programmed to identify a bottle in a scene, grasp it, and pour its "liquid" contents into a cup, requiring coordinated bimanual manipulation and precise flow control.

**Contributions:** I designed and implemented the manipulation architecture and software, developing the kinematics-based motion plans and integrating the dual-arm controller with the higher-level grasping state-machine to ensure reliable object pickup, transport, and pouring.

![S.E.A.L. Team 6](/assets/projects/me326-task3.jpg)

## AA273: Interacting Multiple Model Hand Pose Filtering for Human-Robot Collaboration {#aa273}

**February 2026 – March 2026** | *Stanford, CA*

Human-robot collaboration (HRC) requires robots to accurately predict human intent for both safety and productivity. This project applied an Interacting Multiple Model (IMM) filter to 6-DoF human wrist pose estimation, enabling the robot to distinguish between different motion modes (static, constant velocity, and maneuvering). By soft-switching between these hypothesized modes based on measurement likelihoods, the system utilizes mode probabilities as a proxy for intent.

The IMM filter was validated against standard industrial gestures and achieved 6-DoF tracking accuracy comparable to a Multiplicative EKF (~13.0 mm position and 3.0 degree attitude RMSE) while remaining computationally tractable for real-time use. Crucially, the IMM drastically reduced false-positive detections of abrupt movements by over 80% compared to baseline velocity thresholds, providing a more reliable safety signal for collaborative environments.

**Contributions:** I implemented the IMM filter with "naive mixing" for unit quaternions and performed a comparative analysis against MEKF and QUKF baselines.

## CS229: Machine Learning - Point Cloud Mapping for Pose Estimation of Uncooperative Satellites {#cs229}

**September 2025 – December 2025** | *Stanford, CA*

This project investigated three approaches for mapping point clouds to estimate the pose of uncooperative satellites: a modified iterative closest point (ICP) algorithm, Deep Closest Point (DCP), and a neural network trained with MSE and Chamfer distance losses. As space becomes more crowded, characterizing unknown satellites or space junk by learning their pose and shape is an increasingly critical problem. 

The core innovation involved embedding the FisherRF uncertainty metric into a 3D Gaussian Splatting (3DGS) point cloud model. This allowed for a malleable point cloud mapping that more strongly enforces mappings between points with greater certainty, improving robustness under the noisy and dynamic conditions common in space environments. While classical ICP with FPFH initialization performed well, the study highlighted challenges faced by DCP and neural methods under scale mismatch and indexing variability.

**Contributions:** I implemented the modified ICP and uncertainty-weighted ICP algorithms, and developed the dataset and dataloader infrastructure for the neural network training.

![Proposed Pipeline](/assets/projects/proposed_pipeline.png)

## CS230: Deep Learning - Learning-Based Visuo-Tactile Tendon Perception {#cs230}

**September 2025 – December 2025** | *Stanford, CA*

This project focused on developing a learning-based method for reconstructing contact geometry from vision-based tactile images, specifically for medical applications in identifying the direction and depth of tendons. By analyzing the deformation of a gel membrane "finger," the system aims to provide clinicians with high-fidelity interpretation of subsurface anatomical structures during palpation.

The implemented pipeline utilizes a sequential computer vision approach: a MobileNetV3 for initial object detection, a U-Net for pixel-wise segmentation, and a final U-Net with a frozen DenseNet161 encoder for dense depth reconstruction. The system achieved a classification test accuracy of 0.958 and a depth reconstruction test Mean Absolute Error (MAE) of 4.18mm. The entire pipeline is capable of inferencing in real-time at 12.5Hz, making it suitable for live medical diagnostics.

**Contributions:** I completed the initial manual data labeling for model assessment and implemented the full detection, segmentation, and direction prediction pipeline.

![CS230 Project](/assets/projects/cs230-1.png)

</details>

# University of Cambridge (MPhil Projects)

<details open markdown="1">
<summary><span class="on-close">Click to view Cambridge projects</span><span class="on-open">Collapse Cambridge projects</span></summary>

## MPhil Thesis: Exploring Smartphone-Enabled Gesture Input for Intuitive Robot Teleoperation {#thesis}

**January 2024 – August 2025** | *Cambridge, UK*

One key challenge for robot teleoperation is broadening accessibility beyond specialized users. Many current systems rely on specialist, sometimes expensive, hardware that is not widely available to various groups of users. A promising new direction is the use of everyday devices (e.g., smartphones) as controllers to make teleoperations more affordable and accessible to a broader audience.

To that end, this dissertation involved development and user testing of a hand pose and gesture-based, smartphone-enabled teleoperation system. The system combines the availability of standard consumer technology with the usability, intuitive motion mapping, and lightweight nature of vision-based teleoperation methods. Testing was completed across the Atlantic Ocean, with users in the UK controlling a robot in the US.

The system was developed around the iPhone 14-deployed TeleopLab. This iOS device was chosen as the development platform due to the mass-market adoption of iPhone devices and the TrueDepth camera array. Code was written in Swift 5, with MediaPipe GestureRecognizer used for hand detection and gesture classification. Three gestures enabled tethering the robot to the user’s palm pose, toggling the gripper open and closed, and resetting to a home position. The control system was built on ROS Noetic, with the host computer using the Ubuntu 20.04 OS.

![Thesis Project](/assets/projects/thesis1.png)

## MPhil Student Industrial Consultancy Projects {#consult}

**December 2024 – March 2025** | *Cambridge, UK*

A key part of the MPhil in Industrial Systems, Manufacture, and Management was completion of four industrial consulting projects across England and Wales involving data analysis, process optimization, and strategic recommendations. Three of these projects involved two-week stretches of in-person work with a company, collaborating with a different partner from the cohort each project, where we spoke with operators and management and directly observed processes to generate recommendations. The last project was completed during a term of coursework, so it involved remote collaboration and development of market entry strategy.

### RAM Innovations
The first project was an operations improvement effort at RAM Innovations, an embedded die semiconductor manufacturer in Wales. The company was interested in determining insights for low-cost potential applications of lean manufacturing principles as well as implementation of a rudimentary ERP system for improved stock-keeping.

By conducting interviews and assessing the production halls, we came to conclude that there are improvements needed on seven different elements of the manufacturing operations. We provided an implementation roadmap for usage by the company. We also developed a rudimentary stock-taking system with barcode scanners syncing stock changes during jobs and upon receipt of goods to their (previously manually updated) system to contribute to their digitization efforts.

![RAM Innovations](/assets/projects/ram-1.png)

### 9Barista
This SME based in Cambridge possessed mature operations for production of its flagship product, the 9Barista. However, development of new products during recent years had been slower than desired, and the speed of iteration of integrated prototypes was a particular pain point. The intention of this project was to determine how existing capabilities contribute to design iteration then identify opportunities for improvement. The approach focused on two key elements:

1. Investigation of current R&D process and identification of contributors and detractors to development speed
2. Determination of alterations and enhancements to existing process elements which can create additional speed, especially during design iteration

![9Barista](/assets/projects/9bar-1.png)

As a result of the investigation, three phases were identified as areas of potential improvement: the need for additional structure during product conceptualization and requirements definition, the need to alter project management techniques while planning for the design iteration loop, and the high resource allocation during the fabrication phase. Recommendations were identified which could help to reduce iteration cycles by 5-11 days.

![9Barista 2](/assets/projects/9bar-2.png)

### Huhtamaki BCP
Work-in-progress (WIP) management was a prevalent issue at Huhtamaki BCP. The imbalance of the production line, absence of a WIP tracking system and long dwells of WIP on the shop floor and in the storage areas had led to an elevated WIP pallet congestion problem. It was projected that Huhtamaki BCP is spending £750,000/yr to combat its WIP pallet congestion problem.

The objectives for this project were process-mapping of current WIP storage/flow, identifying factors contributing to high levels of shop floor WIP, and determining WIP pallet storage based on the current situation and future requirements.

![BCP 1](/assets/projects/bcp-1.png)

The approach adopted for this project included Gemba walks, interviews, process and value stream maps and development of solutions from root cause analysis. Solutions were produced to prevent WIP buildup, address WIP tracking and demarcation of storage, and alter the QA hold decision process.

![BCP 2](/assets/projects/bcp-2.png)

The impact of the identified solutions was projected to produce an annual net savings of £450,000 and a 5-day improvement in average lead times.

### SHS One Technologies
The fourth project was completed during the second term of coursework, so one day per week of virtual work was dedicated to this strategy development and market entry strategy project for an early-stage startup.

![SHS](/assets/projects/shs-1.png)

SHS One Technologies, Ltd. (SOT) is a micro-SME planning to apply innovations in advanced hard coatings for industrial applications. Their solution offers superior materials utilization and cycle times compared to current industry standards, but they needed a formal strategy for commercialization. The agricultural and automotive sectors were identified as candidates for initial market entry. This project intended to analyse both markets, formalize a business case, and contextualise critical intellectual property considerations:

1. SOT’s coating technology was analysed to define the unique value proposition and technical feasibility of SHS.
2. A comprehensive market assessment was conducted to identify key opportunities and entry barriers in the agricultural and automotive industries, incorporating market sizing and value chain analysis.
3. Critical insights into market dynamics were obtained by researching the industry and benchmarking the competitors, refining the evaluation of potential business models.
4. Actionable recommendations were formulated to align with SOT’s capabilities, financial constraints and long-term growth objectives through a systematic comparison of market entry strategies.

The key recommendations were confidential given the company’s early-stage state.

</details>

# California Institute of Technology (Undergraduate Projects)

<details open markdown="1">
<summary><span class="on-close">Click to view Caltech projects</span><span class="on-open">Collapse Caltech projects</span></summary>

## ME/CS/EE 134: Robotic Systems - Interactive Robot Backgammon {#backgammon}

**January 2024 – March 2024** | *Pasadena, CA*

In Caltech's ME134 (Robotic Systems), teams of three or four develop a 5-7 degree of freedom (DOF) arm that plays a game or completes an interactive task. My team decided to tackle the challenge of making a robot that you could play backgammon against. While the majority of the challenge in this class was indeed creation of an effective software framework, sound mechanical design was also imperative to achieve millimeter-precise pointing accuracy.

We determined the need for five DOFs because we wanted to manipulate objects both from a "handshaking" wrist position (for grabbing the dice cup) and a "picking" position (for grabbing the checkers and dice). Though we did not end up needing to grab the cup, we still utilized the fourth and fifth DOFs to ensure that our gripper had both the appropriate pitch position to remain parallel to the table and the appropriate yaw position to ensure we only grabbed the intended checker without conflicting against nearby checkers.

![Backgammon](/assets/projects/backgammon2.png)

Both arm links were 450mm long and made of lasercut wood joined into a box to reduce torsional deflection. The equal link length was determined because we wanted to be able to utilize only a single work table and grab checkers on the near side of the board, very close to the base of the robot. Joint brackets were 3D printed PLA.

The initial gripper was designed to grab checkers, dice, and a cup. To handle all of these, it was larger and thicker, which meant that it was more likely to bump into other checkers when attempting to grab one. Once we reduced our scope and swapped to virtual dice rolls, we accordingly modified our gripper to be more specialized for grabbing checkers.

![Backgammon Arm](/assets/projects/backgammon1.png)

For the software, the system consisted of three main ROS nodes. The Detector node was continuously subscribed to the raw camera feed from the top view camera and published the detected position of all checkers and the board. Checkers were detected based on their colors and features, then filtered for existence and correspondence, before finally being sorted based on their positions. The Game node handled the high level playing state of the robot during the game. It generated a set of moves encoded by [source, destination, color] by subscribing to the Detector node’s published game states. This allowed the Game node to always have a real time accurate representation of the current game state.

![Backgammon 4](/assets/projects/backgammon4.png)

Finally, the Trajectory node handled the robot motion planning. It received the location of the checkers and the location of the board from the Detector node, as well as sequences of moves from the Game node. Inverse kinematics were implemented with thresholded singular value decomposition, and trajectory management was handled by queueing six specially defined TaskObjects which atomized different motions. There were no obstacles in the workspace, so task- or joint-space splining between waypoints was a sufficient planning method.

![Backgammon 3](/assets/projects/backgammon3.png)

Beyond creation of the robot and software, we also needed to make a giant backgammon board! We lasercut the board in two halves from the same wood used for the links and laser etched features to aid our painting process. 40mm checkers were 3D printed from PLA and sanded to reduce glare.

![Backgammon 5](/assets/projects/backgammon5.png)

## ME72: Engineering Design Laboratory - Game-Playing Mobile Robots {#me72}

**September 2022 – March 2023** | *Pasadena, CA*

Each year, Caltech ME undergrads form teams of 3-6 to compete in ME72, a capstone engineering design competition. My year, our competition required collecting balls, shooting them into goals, and autonomously navigating an obstacle course with two mobile robots and one stationary shooter.

Our team divided loosely into three sub-teams working on each robot, and I designed and built the shooter robot with a teammate. I designed the shooting tower, articulating turret, structure, and electronics, while he worked on the ball hopper, management, and agitation.

![ME72 5](/assets/projects/me72-5.jpg)

Most of the shooter tower parts were made from waterjet aluminum plate, with some plate bending and other finishing ops. Right before the competition, we opted to replace the shooting curve made from wooden dowels for a 3D printed hood with a smoother profile that gave a more consistent shot. The hood was mounted to a turntable bearing and articulated with a servo-controlled linkage so it could aim at either of two adjacent goals. We used a mix of thick acrylic and thinner plastic sheeting to give the hopper semi-flexible walls.

![ME72 1](/assets/projects/me72-1.png)

Around three weeks before the competition, our team realized that the third robot, which collected and dumped balls into the shooter, was essentially nonfunctional due to poor initial choice of gear reductions. I took on the challenge of fixing the four bar linkage by adding an additional reduction stage, choosing to waterjet these new gears instead of purchasing them and mill the new towers out of leftover stock to minimize downtime. Another teammate fixed the drivetrain, and we were testing again before the end of the week!

![ME72 2](/assets/projects/me72-2.png)

At the final competition, our team placed second. The shooter was extremely reliable, with one wiring mishap that was fixed between rounds with the help of good documentation. My course experience motivated me to be a TA for the following year's competition, "Airship Quadball."

![ME72 3](/assets/projects/me72-3.png)

## LATTICE: Lunar Architecture for Tree Traversal In-service-of Cabled Exploration {#lattice}

**September 2022 – December 2023** | *Pasadena, CA*

At the beginning of my junior year, I returned to campus a month early to work with Caltech Air and Outer Space on the 2022 NASA BIG Idea Challenge. The challenge concerned new methods for maneuvering on the moon, and our idea was a cable-riding shuttle. Most of the ideation was complete by the time I joined the project, so my role was in transitioning the shuttle from concept to product.

I optimized component designs, combining learnings from my summers at Beta with statics knowledge and FEA methods developed through coursework. My modeling, design, and analysis verified adherence to mass and balance requirements before fabrication began.

![LATTICE 1](/assets/projects/lattice-1.png)

The shuttle utilized a self-tensioning design with articulating arms that wrap the cable around the driving pulleys to climb extreme slopes. The carbon fiber tubing used for the shuttle frame allowed it to withstand the extreme tensile forces this caused on the frame. End caps were bonded to the tubes with epoxy, allowing tubes and plates to be bolted together.

Next, I fabricated the gearbox plates and passive outer pulleys for the shuttle. These aluminum plates supported the belt reduction from the motors to the driven pulleys and were designed with functionality and weight savings in mind. These were waterjet out-of-house due to time constraints, with finishing features completed on a manual mill. I also made passive pulleys for the end of the tension arms with a CNC lathe.

![LATTICE 2](/assets/projects/lattice-2.jpg)

Finally, we conducted testing in the Lucerne Valley to validate performance to our intended specifications.

## ME14: Design and Fabrication - Two-Stage Transmission {#me14}

**April 2022 – June 2022** | *Pasadena, CA*

After ME13, in which all ME students at Caltech learn how to use the mill, lathe, lasercutter, waterjet, and 3D printer, ME14 is the first class where we get to take our coursework beyond theory and engineering fundamentals into the shop. We learned fundamentals of GD&T, how to choose motors and other components for mechanical systems, and other engineering best practices (courtesy of Shigley’s).

![ME14 1](/assets/projects/me14-1.jpg)

The main project of our ME14 was a transmission design. Given a motor powered at 12V nominal, a bike wheel load, and a required transmission footprint, we designed a two-stage geared transmission. The plates were milled from acrylic stock, and the shafts were turned from steel shaft stock. Gears were purchased off the shelf.

![ME14 2](/assets/projects/me14-2.png)

I'm always working on something new, whether in or out of the classroom, so stay tuned for new projects!

</details>
