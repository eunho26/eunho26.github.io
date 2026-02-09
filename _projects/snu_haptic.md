---
layout: page
title: SNU-Avatar Haptic Arm
description: A Highly Transparent Operator Interface with Hybrid QDD/DD Actuation for Teleoperation
img: assets/img/Controlroom.jpg
importance: 3
category: paper
related_publications: False
---

> The SNU-Avatar Haptic Arm is a high-performance interface featuring a human-scale workspace that encompasses the full natural range of motion of the upper limb.
> Its hybrid QDD/DD actuation architecture effectively minimizes mechanical resistance to ensure high-fidelity force feedback and precise control.

---

# Abstract
Despite rapid advancements in robotics, teleoperation remains indispensable for precise tasks that have not yet been fully automated. To this end,
this paper presents the design, analysis, and experimental validation of the SNU-Avatar Haptic Arm, a high-performance haptic interface developed for immersive teleoperation. To address the trade-off between transparency and payload capacity, the system employs a hybrid actuation architecture combining quasi-direct drive and direct drive mechanisms. This configuration reduces mechanical impedance and friction while ensuring sufficient force output for high-fidelity interaction. The 6-DoF kinematic structure is designed to encompass the natural workspace of the human upper limb, and finite element analysis confirms that the structural natural frequency is sufficiently high to secure a stable control bandwidth. A comprehensive evaluation validates the system's performance, focusing on force rendering accuracy. The practical utility of the proposed interface was demonstrated in the ANA Avatar XPRIZE Finals through integration with a humanoid robot. The system successfully performed complex missions, such as heavy object manipulation, under constraints including communication latency. The results confirm that the proposed design methodology effectively bridges the gap between remote presence and physical reality, ensuring robust manipulation in extreme environments.

---

# Mechanical Architecture

The **SNU-Avatar Haptic Arm** is a high-performance 6-DoF interface designed to bridge the gap between human operators and remote environments. The system features a human-scale workspace that fully encompasses the natural range of motion of the human upper limb, ensuring unconstrained operation.
This configuration significantly reduces mechanical impedance, enabling precise and immersive dynamic interaction during complex teleoperation tasks.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_01_02.png" title="Overall Joint Configuration" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_01_01.png" title="Kinematic Geometry" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_01_03.png" title="Actuator Module Types" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overall joint configuration, kinematic reference points, and specific actuator module types (QDD/DD) of the proposed haptic arm.
</div>

### **Hybrid Actuation for High Transparency**
To achieve high-fidelity force rendering, the arm employs a specialized hybrid actuation architecture:
* **Shoulder & Elbow (Joints 2–3):** Utilize a 3:1 Quasi-Direct Drive (QDD) pulley transmission to balance torque and backdrivability.
* **Wrist (Joints 4–6):** Implement Direct-Drive (DD) modules to minimize friction and maximize dynamic transparency.
* **Safety & Precision:** Includes a linear prismatic joint with an integrated brake system for stable and secure control.

---

# Design Analysis and Verification

To validate the feasibility of the SNU-Avatar Haptic Arm for practical teleoperation, we conducted a comprehensive analysis across kinematic, dynamic, and structural perspectives. This ensures unrestricted natural motion while maintaining high transparency for physical interaction.

### 1. Workspace Analysis
The device is engineered to encompass the biomechanical range of the human upper limb. Our evaluation confirms that the operational range effectively covers the extensive reachable region of a human operator in both positional and orientation spaces, as illustrated below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_01.png" title="Positional Workspace" class="img-fluid rounded z-depth-1" %}
        <div class="text-center caption">(a) Positional Workspace</div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_02.png" title="Orientation Workspace" class="img-fluid rounded z-depth-1" %}
        <div class="text-center caption">(b) Orientation Workspace</div>
    </div>
</div>
<div class="caption">
    <strong>Figure 1. Workspace validation:</strong> (left) Comparison of the robotic reach with the human workspace, demonstrating a high degree of overlap; (right) Orientation workspace analysis.
</div>

### 2. Force Output Performance
We evaluated the isotropic force distribution and generation capacity, ensuring **sufficient and uniform force output** throughout the nominal workspace. By incorporating advanced gravitational compensation, the system delivers consistent, high-quality haptic feedback with minimal parasitic friction.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_03.png" title="Rated Torque Force" class="img-fluid rounded z-depth-1" %}
        <div class="text-center caption">(a) Under Rated Joint Torques</div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_04.png" %}
        <div class="text-center caption">(b) Under Peak Joint Torques</div>
    </div>
</div>
<div class="caption">
    <strong>Figure 2. Cartesian force capability in the $xy$-plane:</strong> (left) Minimum isotropic force distribution under rated joint torques; (right) Minimum isotropic force distribution under peak joint torques. The black contour indicates the 7 N threshold, with additional reference contours (12 N and 20 N) provided for performance comparison.
</div>

### 3. Structural Modal Analysis
Using Finite Element Method (FEM) simulations, we optimized link lengths to balance workspace requirements with high structural stiffness. This design secures a **wide control bandwidth**, enabling high-fidelity interaction and stable performance without structural resonance.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_05.png" title="Structural Modal Analysis" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <strong>Figure 3. Structural modal analysis results:</strong> Definition of optimized link-length variables ($L_2$, $L_3$) and their corresponding first mode shapes obtained from FEM analysis. The results visualize (a) Link 2 exhibiting a primary bending mode, and (b) Link 3 exhibiting a coupled bending-torsion mode. These modes inform the stiffening strategy to mitigate structural resonance.
</div>


---

