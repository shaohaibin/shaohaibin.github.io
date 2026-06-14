---
layout: page
title: USV Swarm
description:  Unmanned Surface Vehicle Swarm
img: assets/img/projects/USV-swarm/USV-swarm.jpg
importance: 5

category: Swarm
---

<img src="/assets/img/projects/USV-swarm/USV.png" height="550" />

| <img src="/assets/img/images/videos/usv3-1.gif" height="300"  /> | <img src="/assets/img/images/videos/usv6-2.gif" height="300"  /> |

**State-of-the-art**

1. **Distributed Architecture & LPI/LPD Communications**: Shifting from centralized to hybrid “perception-communication-control-decision” architectures. Recent naval exercises (e.g., Silent Swarm 2025) demonstrate smart beam-hopping radios achieving 3× LPI/LPD improvements and 60× instantaneous bandwidth, though 85.4% of studies remain simulation-only.

2. **Adversarial Swarm Intelligence**: Hybrid GAT-Transformer frameworks (Adv-TransAC) enable spatiotemporal meta-reinforcement learning for multi-USV adversarial games, showing emergent cooperative behaviors such as risk-aware interception. Human preference-based RL (RLHF) is also integrated via agent-level binary feedback to encode tacit expert knowledge.

3. **COLREGs-Compliant Collision Avoidance**: CoDAC framework combines cross-modal fusion, incremental dynamic community detection, and an improved velocity obstacle model (IVO-DWA) to achieve 96.7% emergency avoidance success and COLREGs compliance, a 26.7% improvement over traditional methods.

4. **Cross-Domain Heterogeneous Swarms**: Layered “cyber-physical” frameworks (UAV-USV-UUV) demonstrate task decomposition, formation coordination, and low-level control synergy. UAVs provide wide-area surveillance and relay, while USVs act as surface maneuver nodes – however, system-level multi-domain deployment remains unrealized.

5. **Simulation-Centric Validation**: Most USV swarm studies (e.g., using ROS/Gazebo, Unity3D) are confined to virtual environments due to realistic ocean uncertainty, communication dynamics, and safety constraints. System-level sea-trial validation is the most critical bottleneck.

**Future Research Directions**  

1. **Sim-to-Real Bridging & Hybrid Testbeds**: Developing closed-loop validation platforms that integrate real ocean disturbances (nonlinear hydrodynamics, delayed fading channels, sensor noise) with simulation environments to enable continuous, scalable testing from lab to field deployment.

2. **Unified Graph-Signal Processing Framework**: Leveraging graph spectral analysis to tightly couple swarm perception, communication topology, and distributed control – enabling on-the-fly diagnosability of link failures and adaptive task reconfiguration under a single mathematical formalism.

3. **Explainable & Safety-Aware Swarm Learning**: Combining deep reinforcement learning with model predictive control (MPC) and barrier-function-based safe RL to produce verifiable, interpretable decisions for safety-critical missions (e.g., collision-free target interception).

4. **Self-Evolving Adversarial Game Strategies**: Fusing meta-reinforcement learning with game theory to enable rapid adaptation against non-cooperative, dynamically changing opponents. Curriculum learning and mirrored learning are key enablers.

5. **Four-Dimensional (Sea-Land-Air-Undersea) Cross-Domain Integration**: Moving beyond USV-centric formations to full-domain autonomous swarms with semantic-aligned data links, cross-medium communication protocols, and formal guarantees on multi-platform behavioral consistency.

**Challenges**: Real-time onboard LLM/transformer inference, energy efficiency under wave disturbances, scalable verification of emergent swarm behaviors, and mitigation of multi-agent policy hallucinations remain key hurdles. Interdisciplinary efforts combining marine robotics, distributed AI, and hydrodynamic modeling are critical for advancement.