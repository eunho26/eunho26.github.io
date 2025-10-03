---
layout: page
title: SNU-Avatar Robot Hand
description: Dexterous Robot Hand with Prismatic Four-Bar Linkage for Versatile Daily Applications
img: assets/img/hand.jpg
importance: 4
category: paper
related_publications: false
---

> In this work, we introduce a modular robotic hand built on a prismatic four-bar linkage design.
By combining lightweight actuators with a high-stiffness linkage, the hand achieves reliable object grasping and expressive gestures, making it versatile for daily tasks.

---

<!-- Responsive 16:9 wrapper -->
<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;border-radius:12px;">
  <iframe
    src="https://www.youtube-nocookie.com/embed/qNxD-JU64iA?autoplay=1&mute=1&playsinline=1&loop=1&playlist=qNxD-JU64iA&rel=0&modestbranding=1"
    title="YouTube video"
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;"
    allow="autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen
  ></iframe>
</div>

---

# Paper Info
- **Title:** SNU-Avatar Robot Hand: Dexterous Robot Hand with Prismatic Four-Bar Linkage for Versatile Daily Applications
- **Authors:** Eunho Sung, Seungbin You, Seungyeon Kim, Jaeheung Park
- **Keywords:** Robotic Hand, Four-Bar Linkage, Prismatic Joint, Teleoperation, Adaptive Grasping, Modular Design
- **Conference:** IEEE-RAS International Conference on Humanoid Robots (Humanoids)

# Motivation  
- Robotic hands must balance **structural rigidity, sufficient grip force, and adaptability to object shapes** for real-world tasks and teleoperation.  
- Existing designs are often heavy, costly, or difficult to maintain, motivating the development of a **lightweight, modular, and affordable hand with robust performance**. 

# Key Contributions  
- Introduces a **prismatic four-bar linkage structure** that enables MCP–PIP–DIP flexion with a single linear actuator.  
- Combines **adduction/abduction (AA) joints with springs** to achieve compliant and adaptive grasping.  
- Proposes a **modular finger design** (4 fingers, 8 DoF) for easy maintenance and replacement.  
- Validates design through **FEM analysis and experiments**, demonstrating robustness against external loads.  
- Shows capability to perform a wide range of **grasp taxonomy motions and expressive gestures**.  

# Hardware at a Glance  
- **Size/Weight:** 211.5 mm height, 70 mm width, 832 g.  
- **Degrees of Freedom:** 4 fingers × (FE + AA) = 8 DoF total.  
- **Actuators:** ROBOTIS Dynamixel (XC330 series) smart actuators.  
- **Materials:** Aluminum + S45C (reinforced at critical joints) + 3D-printed parts.  
- **Special Features:** Silicone fingertip pads and a curved palm for increased friction and contact stability.  

# Working Mechanism  
- **Flexion/Extension (FE):** Driven by a lead screw integrated with a prismatic four-bar linkage, enabling high stiffness and efficient force transmission.  
- **Adduction/Abduction (AA):** Independent motor actuation with preload springs, supporting adaptive grasping and gesture expression.  
- **Kinematics:** Closed-form equations derived from link lengths, angles, and screw displacement allow precise calculation of fingertip trajectories and joint angles.  
- **Structural Reliability:** FEM analysis confirmed improved safety factor (7.2) and reduced displacement when replacing aluminum with S45C at load-critical joints.  

# Takeaway: 
This work presents a **lightweight, modular, and cost-effective robotic hand** that combines high stiffness, grip strength, and compliance.  
Validated through both simulation and experiments, the hand demonstrates reliable daily object manipulation and expressive gesture capabilities, offering strong potential for **teleoperation and service robotics applications**.  

**BibTeX**

```bibtex
@inproceedings{Sung2025SNUAvatarGlove,
  author={Sung, Eunho and You, Seungbin and Kim, Seungyeon and Park, Jaeheung},
  booktitle={2023 IEEE-RAS 22nd International Conference on Humanoid Robots (Humanoids)}, 
  title={SNU-Avatar Robot Hand: Dexterous Robot Hand with Prismatic Four-Bar Linkage for Versatile Daily Applications}, 
  year={2023},
  pages={1-8},
  keywords={Couplings;Avatars;Taxonomy;Humanoid robots;Finite element analysis;Timing;Task analysis},
  doi={10.1109/Humanoids57100.2023.10375222}
}
``` 
