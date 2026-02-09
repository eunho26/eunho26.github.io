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
        {% include figure.liquid loading="eager" path="assets/img/Haptic_01_02.png" title="Overall Joint Configuration" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_01_01.png" title="Kinematic Geometry" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_01_03.png" title="Actuator Module Types" class="img-fluid" %}
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
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_01.png" title="xy-position workspace" class="img-fluid" %}
        <div class="text-center caption">(a) xy-position workspace</div>
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_06.png" title="3D position workspace" class="img-fluid" %}
        <div class="text-center caption">(b) 3D position workspace</div>
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_02.png" title="Direction vectors" class="img-fluid" %}
        <div class="text-center caption">(c) Achievable direction vectors on the unit sphere</div>
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_07.png" title="Psi bounds" class="img-fluid" %}
        <div class="text-center caption">(d) Corresponding $\psi$ bounds in the $(\theta,\phi)$ parameter space</div>
    </div>
</div>
<div class="caption">
    <strong>Figure 1. Comprehensive workspace validation:</strong> (a-b) Positional reach in 2D and 3D spaces, and (c-d) orientation analysis including feasible rotation ranges on a unit sphere and their corresponding parameter bounds.
</div>

### 2. Force Output Performance
We evaluated the isotropic force distribution and generation capacity, ensuring **sufficient and uniform force output** throughout the nominal workspace. By incorporating advanced gravitational compensation, the system delivers consistent, high-quality haptic feedback with minimal parasitic friction.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_03.png" title="Rated Torque Force" class="img-fluid" %}
        <div class="text-center caption">(a) Under Rated Joint Torques</div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_04.png" title="Rated Torque Force2" class="img-fluid" %}
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
        {% include figure.liquid loading="eager" path="assets/img/Haptic_02_05.png" title="Structural Modal Analysis" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    <strong>Figure 3. Structural modal analysis results:</strong> Definition of optimized link-length variables ($L_2$, $L_3$) and their corresponding first mode shapes obtained from FEM analysis. The results visualize (a) Link 2 exhibiting a primary bending mode, and (b) Link 3 exhibiting a coupled bending-torsion mode. These modes inform the stiffening strategy to mitigate structural resonance.
</div>


---

# Experimental Validation & Field Testing

To demonstrate the effectiveness of the proposed 6-DoF haptic interface, we conducted a phased verification process ranging from fundamental hardware benchmarking to field validation in the ANA Avatar XPRIZE Finals.

### 1. Fundamental Hardware Performance
First, we evaluated the open-loop force rendering capability to ensure the haptic device could generate precise and repeatable forces. The evaluation across 40 trials at four force levels (2.5–10.0 N) demonstrated high repeatability with low standard deviations (0.093–0.367 N), confirming consistent force generation. While a slight steady-state bias was observed at higher magnitudes, the concentrated force distributions verify the system's reliability for stable haptic rendering in open-loop operations.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_03_01.png" title="Experimental Setup" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_03_02.png" title="Force Repeatability" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Haptic_03_03.png" title="Operator Configuration" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    <strong>Experimental validation and system configuration.</strong> 
    From left to right: the experimental setup for open-loop force evaluation using a 6-axis F/T sensor, the resulting force rendering repeatability across target levels, and the operator-side hardware layout including the bimanual haptic setup and tracking system.
</div>

### 2. Teleoperation System Integration
We integrated the haptic arm with the humanoid robot TOCABI to verify basic teleoperation performance. The system was tested under a realistic network architecture to assess stability.

#### Remote Pick-and-Place Demonstration
The practical utility of the system was verified through a remote pick-and-place sorting task. The operator successfully grasped and placed eight objects into two containers using the haptic feedback.

#### Field Validation: ANA Avatar XPRIZE
Finally, to assess applicability in unpredictable real-world environments, we analyzed the performance during the **ANA Avatar XPRIZE Finals**. The system was tested under extreme conditions characterized by restricted fields of view and communication delays.

The haptic feedback played a crucial role in completing complex missions, such as:
* **Mission 4:** Activating a switch with precise force control.
* **Mission 6 & 7:** Distinguishing and manipulating heavy canisters (weight perception).
* **Mission 9:** Utilizing a power drill (vibration feedback).
