---
layout: page
title: ANA Avatar Xprize
description: with background image
img: assets/img/Avatarxprize.jpg
importance: 2
category: project
related_publications: false
---

> TEAM SNU developed an intuitive robotic avatar system using the TOCABI humanoid and a mobile base, enabling natural full-body teleoperation through multi-modal feedback. In the ANA Avatar XPRIZE finals, the system successfully completed 8 out of 10 missions and ranked 8th among 17 teams.

---

<!-- Responsive 16:9 wrapper -->
<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;border-radius:12px;">
  <iframe
    src="https://www.youtube-nocookie.com/embed/rehGcSoCrSU?autoplay=1&mute=1&playsinline=1&loop=1&playlist=rehGcSoCrSU&rel=0&modestbranding=1"
    title="YouTube video"
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;"
    allow="autoplay; encrypted-media; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen
  ></iframe>
</div>
---

# Project Progress and Competition Results

## Background

TEAM SNU advanced to both the semifinals and finals of the ANA Avatar XPRIZE. In the 2021 semifinals held in Miami, Florida, the team demonstrated full-body motion retargeting and remote operation capabilities, thereby securing a place in the finals. The finals took place over four days in November 2022 in Long Beach, California, where 17 finalist teams competed in completing 10 standardized missions.

## Competition Format

Each team was assigned two operators who, after a brief training session, carried out the missions. The tasks included object manipulation, object transportation, cooperative interactions, navigation, and obstacle avoidance. TEAM SNU employed the TOCABI humanoid robot with a mobile base as the avatar platform, integrating HMDs, haptic devices, trackers, gloves, and pedals to realize multi-modal feedback–based full-body teleoperation.

## Results

The team successfully completed 8 out of 10 missions and placed 8th among the 17 finalist teams. Their system received positive evaluations for its ability to integrate precise manipulation with mobility, enable natural full-body teleoperation, and allow intuitive operation even after minimal training. However, limited preparation time and certain hardware constraints prevented the completion of all missions.

## Significance

The project demonstrated the feasibility of an avatar system that can be intuitively operated in complex remote environments. This achievement highlights the potential for real-world applications in areas such as disaster response, healthcare and caregiving support, and remote industrial operations.

{% include figure.liquid
   loading="eager"
   path="assets/img/snu002.jpg"
   title="example image"
   class="img-fluid rounded z-depth-1"
%}

---

# Remote-Side Robot System

The remote side of the avatar system is composed of the **humanoid robot TOCABI** and the **SNU-Avatar Robot Hand**.  
Together, they provide whole-body mobility and dexterous manipulation for immersive teleoperation.

## TOCABI (Humanoid Robot)

- Height / Weight: **1800 mm, 100 kg**
- Degrees of Freedom: **33 DoF (2 + 16 + 3 + 12)**
- Reduction Ratio: **100:1**

**Related Publications**

- Park, Beomyeong, et al. _“Intuitive and Interactive Robotic Avatar System for Tele-Existence: TEAM SNU in the ANA Avatar XPRIZE Finals.”_ International Journal of Social Robotics, 2024.
- Park, Beomyeong, et al. _“Team SNU’s avatar system for teleoperation using humanoid robot: ANA Avatar XPRIZE competition.”_ RSS Workshop on “Towards Robot Avatars,” 2022.
- Schwartz, Mathew, et al. _“Design of the humanoid robot TOCABI.”_ Humanoids, IEEE, 2022.

## SNU-Avatar Robot Hand

- **Configuration:** 4 modular fingers, 8 DoF total
- **Mechanism:** Prismatic four-bar linkage for MCP–PIP–DIP flexion
- **Adaptation:** Adduction/abduction with springs for compliant grasping
- **Structure:** Lightweight design (832 g) using aluminum, S45C, and 3D-printed parts
- **Features:** Silicone fingertip pads + curved palm for stable and adaptive contact
- **Validation:** FEM analysis and experiments confirm robustness against external loads

**Related Publications**

- Eunho Sung, et al. _“SNU-Avatar Haptic Glove: Novel Modularized Haptic Glove via Trigonometric Series Elastic Actuators.”_ IROS, IEEE, 2024.
- Seungyeon Kim, et al. _“3-finger robotic hand and hand posture mapping algorithm for avatar robot.”_ Journal of Korea Robotics Society.

## Mobile Platform

- **Type:** Mecanum wheel-based mobile platform
- **Purpose:** Designed to carry TOCABI in a seated position, primarily for manipulation tasks
- **Advantage:** Overcomes limitations of humanoid walking by combining a humanoid robot with a wheeled base
- **Application:** Enhances mobility in telepresence scenarios, allowing navigation across diverse environments and improving task efficiency

**Related Publications**

- Lim, Daegyu, et al. _“Foot-Operated Telelocomotion Interface for Avatar Robots Utilizing Mecanum Wheel-based Mobile Platforms.”_ ICCAS, 2023.

{% include figure.liquid
   loading="eager"
   path="assets/img/snu001.jpg"
   title="example image"
   class="img-fluid rounded z-depth-1"
%}

---

# Operator-Side System

The operator station provides intuitive control and immersive feedback to enable natural teleoperation of the avatar robot. It integrates visual, haptic, and motion-tracking systems to ensure seamless coordination with the remote humanoid.

## System Components

- **Tracking:** Vive Base Station + Vive Tracker 3.0
- **Vision/HMD:** Vive Pro 2 (HMD)
- **Haptics:** DYROS Haptic Arms + Haptic Gloves

## SNU-Avatar Haptic Glove

- **Configuration:** 4 modular finger units (thumb, index, middle, ring)
- **Mechanism:** Trigonometric SEA for force feedback with reduced encoders
- **Mounting:** Middle-phalanx attachment with fingertip estimation
- **Design:** Rigid exoskeletal frame, Boa fitting, Arduino-based I/O, add-on ready
- **Validation:** Force accuracy, fingertip estimation, and Grasp Taxonomy tests

**Related Publications**

- Eunho Sung, et al. _“SNU-Avatar Robot Hand: Dexterous Robot Hand with Prismatic Four-Bar Linkage for Versatile Daily Applications.”_ Humanoids, IEEE, 2023.
- Suhan Park, et al. _“Operator-Avatar Texture Feedback Approach using Hand-eye Camera and Force Sensor.”_

## Vision / HMD

Vision is the most critical feedback channel in the avatar system. A smooth and realistic visual experience enhances operator immersion and task performance.

- **Coherent Field of View:** Robot head (TOCABI) synchronized with HMD orientation
- **Depth Perception:** Dual cameras fused in Unity for stereoscopic vision
- **Low Latency:** 0.2–0.4 sec delay (camera → HMD) achieved via TCP streaming
- **Feedback Cues:** Weight estimation and grasping feedback delivered visually
- **Intuitive UI Design:** Tailored to support operator awareness and precision

**Related Publications**

- Shin, Jaeyong, et al. _“Virtual Reality Based Intuitive Spatial Visual Interface for Avatar Robot System.”_ ICCAS, IEEE, 2023.
- Shin, Jaeyong, et al. _“Stereoscopic low-latency vision system via ethernet network for humanoid teleoperation.”_ UR, IEEE, 2022.

## Expressing Emotion

Conveying the operator’s intention and emotion is essential for natural communication in avatar telepresence.

- Operator’s **voice** captured via HMD microphone and transmitted to TOCABI speakers
- **5-inch LCD display** mounted on the robot mouth to visualize emotional expressions
- Animations generated using **Google NLP API**, which recognizes emotion in operator’s voice

**Related Publications**

- Schwartz, Mathew, et al. _“Design and Control of a Humanoid Avatar Head with Realtime Face Animation.”_ ICCAS, IEEE, 2022.

## Motion Retargeting

The avatar robot reproduces the operator’s body movements, adapting them to its own morphology and dynamic constraints.

- **Human posture** tracked via Vive Trackers
- **Task Prioritization:** Dynamic behaviors generated depending on situational priorities
- **Optimization-based IK:** Inverse kinematics controller maintains robot balance and executes manipulation tasks simultaneously

**Related Publications**

- Lim, Daegyu, et al. _“Online telemanipulation framework on humanoid for both manipulation and imitation.”_ UR, IEEE, 2022.

{% include figure.liquid
   loading="eager"
   path="assets/img/snu003.jpg"
   title="example image"
   class="img-fluid rounded z-depth-1"
%}
