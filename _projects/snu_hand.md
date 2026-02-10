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
> By combining lightweight actuators with a high-stiffness linkage, the hand achieves reliable object grasping and expressive gestures, making it versatile for daily tasks.

---

# Abstract
This paper presents an innovative approach to designing a robot hand specifically tailored for the final round of the ANA Avatar XPRIZE Challenge, a teleoperation robot competition. The primary objective of the newly developed hand was to accurately depict teleoperation by replicating a person's remote actions, gestures, emotional expressions, and the ability to manipulate various objects commonly encountered in daily life, including tools. To accomplish the objective of enabling finger flexion-extension (FE) with a single linear actuating system, multiple 4-bar linkage mechanisms were employed to incorporate the FE joints. Additionally, to enable effortless grasping of objects with unknown shapes, compliance elements were implemented using adduction-abduction (AA) joints with timing belt pulley system and FE joint accompanying springs. As a result, a four-fingered hand boasting a total of eight degrees of freedom was developed, ensuring robust fingertip grip while minimizing the overall weight of the hand to preserve the payload capacity of the robot arm. This paper describes the hand's design process based on finger kinematic analysis. Finite Element Method (FEM) analysis results to assess the hand's ability to withstand disturbances and potential plastic deformation. Furthermore, taxonomy analysis derived from real gripping experiments.

---

# High-Rigidity Telepresence Robot Hand

Designed with the rigorous demands of the **ANA Avatar XPRIZE** in mind, this **8-DoF robot hand** is optimized for immersive telepresence and high-load task execution. The structure prioritizes **rigidity and grip strength**, enabling it to withstand **40N** of force during lever pulls and secure **2kg** payloads without deformation. By integrating a robust **4-finger configuration** with easy-to-maintain smart actuators, this platform delivers the mechanical resilience and precision necessary for reliable, real-time remote interaction in extreme competition scenarios.

{% include figure.liquid loading="eager" path="assets/img/Hand_01_01.png" title="Hand_01_01" class="img-fluid" %}

---
# Modular & High-DoF Design for Versatile Grasping

<div class="row align-items-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        <p>
            The robot hand features a modular four-finger configuration—comprising the thumb, index, middle, and ring fingers—that provides 8 degrees of freedom (8 DoF) through independent actuation. Each finger is driven by separate Flexion/Extension (FE) and Adduction/Abduction (AA) actuators, allowing for the precise and complex manipulation required for versatile tasks.
        </p>
        <p>
            Designed for both durability and performance, the hand measures 211.5 mm in height and 70 mm in width, weighing 832 g due to its composite structure of aluminum, iron, and 3D-printed parts. It supports a maximum grasping width of 165 mm at full extension, with silicon pads strategically integrated onto the fingertips and knuckles to ensure enhanced stability and secure contact with objects.
        </p>
    </div>

    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_01_02.png" class="img-fluid" title="Modular Finger Design and Linkage Structure" %}
    </div>
</div>

---
# Modular Architecture for Adaptive and High-Fidelity Grasping

The robot hand features a modular four-finger architecture powered by compact smart actuators, ensuring exceptional ease of maintenance and seamless individual finger replacement. Its performance is optimized through integrated mechanical springs that enable compliant and adaptive motion, allowing the hand to securely conform to objects of diverse shapes. Enhanced by high-friction silicone fingertips and a strategically curved palm, the design maximizes contact area and grip stability for reliable interaction in complex teleoperation environments.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_02_01.png" class="img-fluid" title="Hand_02_01" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_02_02.png" class="img-fluid" title="Hand_02_02" %}
    </div>
</div>

<div class="row">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_02_03.png" class="img-fluid" title="Hand_02_03" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_02_04.png" class="img-fluid" title="Hand_02_04" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_02_05.png" class="img-fluid" title="Hand_02_05" %}
    </div>
</div>

---

# Anthropomorphic Finger Design and High-Precision Linkage Mechanism

The robot finger is meticulously designed with a five-link, four-joint structure that closely mirrors human anthropometry, featuring proximal, middle, and distal phalanx segments of 40 mm, 28 mm, and 27.5 mm respectively to replicate natural grasping motions. Each 180g module integrates an Adduction/Abduction (AA) actuator in the base and a Flexion/Extension (FE) actuator within a middle link, where a specialized crank-slide configuration converts linear lead screw motion into precise joint rotation across the MCP, PIP, and DIP joints. This biomimetic approach, combined with a compact 171 mm module length, ensures that the robot hand can achieve the dexterity and structural resilience necessary for complex teleoperation tasks while maintaining a form factor familiar to human users.

{% include figure.liquid loading="eager" path="assets/img/Hand_01_03.png" title="Hand_01_03" class="img-fluid" %}

---

# Optimized Structural Durability and Validated Grasping Performance

To withstand the 40 N force required for high-load tasks like the ANA Avatar XPRIZE lever pull, we optimized the MCP-FE joint using Finite Element Method (FEM) analysis. Replacing the original aluminum frame with high-strength S45C (AISI 1045) steel significantly increased the safety factor from 1.307 to 7.201. This modification reduced maximum displacement to just 0.0735 mm, ensuring the hand remains resilient against plastic deformation under extreme operational loads.

The practical grasping capability was validated through pinch grasping experiments, representing the most stringent conditions where force distribution is absent. In cyclic tests approximating real-world contact, the finger consistently demonstrated an output force averaging 4.92 N at an actual current of approximately 650 mA. These results confirm the robot hand's ability to maintain a secure grip, proving the design is fully capable of executing complex manipulation tasks with high fidelity.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_03_01.png" class="img-fluid" title="Hand 01-01" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_03_02.png" class="img-fluid" title="Hand 03-02" %}
    </div>
</div>

---

# Versatile Grasping Capabilities and Expressive Non-Verbal Communication

{% include figure.liquid loading="eager" path="assets/img/Hand_03_03.png" title="Hand_03_03" class="img-fluid" %}

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
{% include figure.liquid loading="eager" path="assets/img/Hand_01_03.png" title="Hand_01_03" class="img-fluid" %}
- Robotic hands must balance **structural rigidity, sufficient grip force, and adaptability to object shapes** for real-world tasks and teleoperation.
- Existing designs are often heavy, costly, or difficult to maintain, motivating the development of a **lightweight, modular, and affordable hand with robust performance**.



# Key Contributions

<div class="row align-items-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        <p>
            This research presents a novel robotic hand design featuring a <strong>prismatic four-bar linkage structure</strong>, which effectively facilitates MCP–PIP–DIP flexion using only a single linear actuator. To enhance grasping versatility, the design integrates <strong>adduction/abduction (AA) joints equipped with springs</strong>, enabling compliant and adaptive interactions with various objects. 
        </p>
        <p>
            The system employs a <strong>modular finger architecture</strong> (comprising 4 fingers and 8 Degrees of Freedom) to ensure ease of maintenance and component replacement. The structural integrity of the design is validated through rigorous <strong>FEM analysis and experimental trials</strong>, proving its robustness against significant external loads. Ultimately, the proposed mechanism demonstrates superior performance across a broad spectrum of <strong>grasp taxonomy motions</strong> and highly expressive gestures.
        </p>
    </div>

    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_01_02.png" class="img-fluid" title="Modular Finger Design and Linkage Structure" %}
    </div>
</div>

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

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_03_01.png" class="img-fluid" title="Hand 01-01" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hand_03_02.png" class="img-fluid" title="Hand 03-02" %}
    </div>
</div>

# Takeaway:

This work presents a **lightweight, modular, and cost-effective robotic hand** that combines high stiffness, grip strength, and compliance.  
Validated through both simulation and experiments, the hand demonstrates reliable daily object manipulation and expressive gesture capabilities, offering strong potential for **teleoperation and service robotics applications**.

{% include figure.liquid loading="eager" path="assets/img/Hand_03_03.png" title="Hand_03_03" class="img-fluid" %}

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
