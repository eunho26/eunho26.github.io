---
layout: page
title: Plate Harmonic Reducer
description: Profiled Groove Wave Generator
img: assets/img/PHRth.jpg
importance: 3
category: project
related_publications: true
---

This project, led by **Seungbin You**, focuses on the design and development of a Plate Harmonic Reducer.  
In addition, we have completed a follow-up study that further advances this concept by emphasizing the unique advantages demonstrated in the original results, and we are currently preparing for its presentation.  

---
> This study introduces a plate-type harmonic reducer as a novel alternative to conventional cup-type designs, achieving reduced axial thickness, increased torsional stiffness, and significantly lower deformation force. By implementing a **profiled-groove wave generator** and a split flexspline design, the work verifies both theoretical feasibility and practical realizability, demonstrated through a 3D-printed prototype experiment.

---
# Paper Info
- **Title:** Plate Harmonic Reducer with a Profiled Groove Wave Generator
- **Authors:** Seungbin You, Jaesug Jung, Eunho Sung, Jaeheung Park
- **Keywords:** Harmonic Reducer, Plate Harmonic Reducer (PHR), Wave Generator, Flexspline, Robotics Actuator
- **Conference:** 2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)

# Motivation  
Conventional harmonic reducers (HRs) are widely adopted in robotic actuators for their compact size, zero backlash, and high precision.  
However, they face inherent limitations such as **minimum axial thickness**, **relatively low torsional stiffness**, and **high deformation force requirements**.  
To overcome these drawbacks, this work introduces a **Plate Harmonic Reducer (PHR)**, which reconfigures the cup-type flexspline into a thin plate form.  

# Key Contributions  
- Proposes a **plate-type flexspline (FS)** that enables slimmer axial packaging compared to conventional cup-type HRs.  
- Introduces a **profiled-groove wave generator (WG)** with steel balls and cage, achieving **low-friction rolling contact** and **adjustable tooth engagement ratio**.  
- Develops a **split FS design** to alleviate stress concentration and reduce deformation force.  
- Validates performance improvements via FEM and experiments: **~8× lower deformation force** and **>4× higher torsional stiffness**, while demonstrating operational feasibility with a 3D-printed prototype.  

# Hardware at a Glance  
- **Outer diameter:** 90 mm  
- **Reduction ratio:** 50:1 (100/102 teeth)  
- **Weight:** 175 g (3D-printed prototype, Tough PLA)  
- **Wave generator:** Steel balls + cage with profiled groove  
- **Actuation:** Maxon BLDC motor (180 W) with dual encoders (131,072 CPR and 983,040 CPR)  
- **Housing:** High-stiffness structure assembled with M3 bolts  

# Working Mechanism  
- The **profiled groove wave generator** displaces steel balls along its contour, deforming the plate-type flexspline (FS) **axially at specific contact points**.  
- The deformed FS engages with the circular spline (CS), producing **reverse-direction, high-ratio reduction** of the input motion.  
- The rolling-contact mechanism minimizes friction, while the groove profile allows tuning of the tooth engagement ratio to increase torque capacity.  

# **Takeaway:**  
The Plate Harmonic Reducer (PHR) represents a **new structural paradigm** in strain-gear technology:  
- **Thinner axial geometry**  
- **Higher torsional stiffness**  
- **Lower deformation force**  

while retaining the hallmark benefits of harmonic drives.  
This makes the PHR a strong candidate for **compact, high-performance robotic actuators** in next-generation systems.  
