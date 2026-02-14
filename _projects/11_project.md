---
layout: page
title:  UAV Swarm Hunter
description: UAV Hunter
img: assets/img/projects/netgun-UAV/netgun-UAV.png
importance: 5
category: Swarm
---


| <img src="/assets/img/projects/netgun-UAV/netgun-uav-1.gif" height="250" /> | <img src="/assets/img/projects/netgun-UAV/netgun-uav-2.gif" height="250" /> |

| <img src="/assets/img/projects/netgun-UAV/netgun-UAV.png" height="250" /> |  <img src="/assets/img/projects/netgun-UAV/UAV-hunter-target.jpg" height="250" /> |

**State-of-the-art**

1. Early Development: Initial systems relied on a single interceptor drone manually controlled by a ground operator to fire a capture net. Success rates were heavily dependent on operator skill.

2. Autonomous Interception: Recent advancements integrate onboard vision systems and predictive control. For instance, Zheng et al. (2025) demonstrated a vision-based autonomous system where a quadcopter tracks a target using onboard cameras and triggers the net via Model Predictive Control (MPC), achieving a 64.7% success rate in real-world tests.

3. Cooperative Capture: To intercept high-speed targets, projects like the EU's MIDRAS have developed multi-drone systems. Multiple UAVs collaboratively carry and deploy a single large net, using centralized path planning and formation control. This approach has successfully demonstrated the capability to intercept targets moving at up to 30 m/s.

**Future Research Directions**

1. AI-Driven Autonomous Decision-Making: Moving beyond simple tracking to incorporate deep learning for intent prediction and tactical planning. AI will enable the interceptor to anticipate a target's maneuvers and choose the optimal capture strategy in real-time.

2. Cooperative Swarm Capture: Developing advanced swarm algorithms for multi-agent systems to cooperatively capture multiple targets simultaneously. This includes research into "swarm vs. swarm" tactics and distributed intelligence.

3. Flexible and Adaptive Capture Mechanisms: Moving beyond rigid nets to develop adaptive capture devices, such as morphing nets or tethered grappling mechanisms, that can effectively secure targets of varying sizes and shapes in different flight conditions.

4. Integration with Layered Defense Systems: Net-capture drones will not operate in isolation. Future systems will be seamlessly integrated into a layered defense architecture, working in concert with radar networks, RF detectors, and other countermeasures for a coordinated and proportionate response.

** Key Challenges**

1. High-Speed & Agile Target Interception: Current systems struggle with fast and unpredictably maneuvering targets like racing drones (FPVs), which can exceed speeds of 30 m/s with rapid acceleration changes.

2. Environmental Reliability: The performance of vision-based systems degrades significantly in adverse weather conditions (rain, fog, low light), and radar can be ineffective against small, low-speed drones. Ensuring 24/7 reliability remains a hurdle.

3. Operational Safety: Deploying a high-speed interceptor in public or sensitive areas carries inherent risks. Ensuring the net-capture system itself does not become a hazard (e.g., through collision or falling debris) is a critical safety and regulatory concern.

4. Scalability and Swarm vs. Swarm: Coordinating multiple friendly drones to capture a single rogue drone is complex. The challenge is exponentially greater when facing a coordinated swarm of hostile drones.