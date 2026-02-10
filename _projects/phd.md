---
layout: page
title: Plate Harmonic Reducer
description: Profiled Groove Wave Generator
img: assets/img/PHRth.jpg
importance: 3
category: project
related_publications: false
---

This project, led by **[Seungbin You](https://scholar.google.co.kr/citations?user=14WuFEkAAAAJ&hl=ko)**, focuses on the design and development of a Plate Harmonic Reducer.  

Conventional harmonic drives, while precise, suffer from bulky axial lengths and efficiency drops at lower reduction ratios. This research series introduces a breakthrough **Axial Deformation mechanism**, transforming the traditional cup-shaped gear into a flat, plate-like form. By leveraging Kirchhoff-Love plate theory and innovative contact geometries, these studies provide a complete roadmap from theoretical invention to industrial optimization.

---

### Revolutionizing Robotic Actuation: The Next-Gen Plate Harmonic Reducer (PHR)

As robotics demand increasingly compact, lightweight, and high-precision components, traditional speed reducers are hitting their physical limits. Our research team presents a paradigm shift in strain wave gearing through a series of **three pivotal studies** on the **Plate Harmonic Reducer (PHR)**—a novel architecture that redefines the standards for robotic joint modules.

{% include figure.liquid loading="eager" path="assets/img/PHD_01_02.png" title="PHD_01_02" class="img-fluid" %}

---

### Evolution of the Research (3 Key Publications)

##### 1. Structural Innovation: Realizing the Plate Form
The foundational study introduces the PHR’s unique topological structure. Unlike conventional strain gears that deform radially, the PHR utilizes **axial elastic deformation**. Through Finite Element Method (FEM) and 3D-printed prototyping, this research proves that the PHR can maintain "backlash-free" precision while significantly reducing the motor's overall footprint.

##### 2. Performance Gap Solution: The Tri-contact System (Tri-c PHR)
Robotic actuators often struggle in the "mid-range" reduction ratios (around 16:1). This second study presents the **Tri-contacted Plate Harmonic Reducer**, which employs a three-point tooth engagement system. This design achieves a **16:1 ratio**—a zone where traditional harmonic drives face design challenges—offering high torque transparency and backdrivability comparable to premium commercial units.

##### 3. Mechanical Optimization: Ultra-Thin Performance
The final study provides a comprehensive mechanical analysis of the PHR's thickness-to-performance relationship. By optimizing the plate to an ultra-thin **0.4mm** configuration, we achieved:
* **40.3% Reduction** in axial thickness.
* **27.2% Reduction** in total weight.
* **68.8% Transmission Efficiency**, matching commercial standards.
This paper establishes validated design guidelines, balancing the trade-off between ultra-thin efficiency and torsional stiffness.

---

# Plate Harmonic Reducer with a Profiled Groove Wave Generator

In this study, a mechanism that realizes a novel structural form of the harmonic reducer is introduced. Conventional robots often use various mechanical reducers owing to low torque and high-speed characteristics of electric motors. Among them, harmonic reducers are frequently used because of their compact size and backlash-free precision. The plate harmonic reducer which uses the same topological geometry and reducing mechanism as the conventional harmonic reducer is a novel type of strain gear that changes its shape to a plate form for axial deformation. It has unique differences in terms of axial thickness, torsional stiffness, and efficiency due to its morphological characteristics. This study introduces and analyzes the reducing principle of the plate harmonic reducer and describes the methodological solutions for realization. Finally, the theoretical performance improvement and operating feasibility of the plate harmonic reducer are analyzed using finite element method and a 3D-printed prototype model.

---

## Plate Harmonic Reducer (PHR): Axial-Meshing, High-Ratio Single-Stage Reduction

Inspired by the conventional harmonic reducer, the Plate Harmonic Reducer (PHR) achieves high reduction by continuously shifting the meshing state between a flex spline (FS) and a circular spline (CS). Unlike radial meshing in standard designs, the PHR uses **axial meshing teeth** and a specially designed wave generator (WG) that **pushes the plate-shaped FS in the axial direction** at the contact points. As the WG rotates under input torque, the engagement regions travel around the splines, forcing the FS to rotate in the opposite direction at a reduced speed—delivering high torque density in a compact, single-stage architecture. By axially fixing the housing and CS, the WG maintains consistent deformation force, while the FS transfers the reduced-speed output torque. Because axial tooth pressure continuously loads the housing, **housing support stiffness becomes a critical design driver**, complemented by ball-and-cage elements to minimize friction.


{% include figure.liquid loading="eager" path="assets/img/PHD_01_01.png" title="PHD_01_01" class="img-fluid" %}

---

## Advanced WG Profiling & Contact Mechanics

This study optimizes torque transmission through advanced Wave Generator (WG) profiling, demonstrating how cubic spline functions outperform linear designs by maximizing tooth contact ratios. By modeling the engagement mechanism as a modified rack-and-pinion system, we provide a detailed free-body analysis that accurately derives axial loads and friction dynamics. This framework ensures precise control over harmonic elastic deformation, utilizing optimized trapezoidal and involute tooth geometries for superior mechanical efficiency.

{% include figure.liquid loading="eager" path="assets/img/PHD_01_03.png" title="PHD_01_03" class="img-fluid" %}

---

## FEM Validation: Superior Stiffness & Structural Efficiency

Validated through rigorous FEM analysis, the PHR architecture demonstrates superior structural efficiency compared to conventional Harmonic Reducers. Our simulation reveals a radical improvement in elastic mechanics, requiring eight times less force to achieve the necessary deformation. Furthermore, the PHR exhibits exceptional torsional rigidity, maintaining minimal displacement under high-torque conditions to ensure precision and stability in demanding applications.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/PHD_01_04.png" title="PHD_01_04" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/PHD_01_05.png" title="PHD_01_05" class="img-fluid" %}
    </div>
</div>

---

## Rigorous Experimental Validation: Precision & Efficiency

To validate the PHR's real-world performance, we conducted comprehensive comparative testing against industry-standard Harmonic Reducers (SHG-17-50-2SH). Our transmission error analysis confirmed high positional fidelity, while dynamic load testing demonstrated that the 3D-printed prototype achieves a promising 55.72% efficiency across varying speeds. These results not only verify the reliability of our experimental setup against established benchmarks but also prove the practical viability of the PHR architecture for precision motion applications.

{% include figure.liquid loading="eager" path="assets/img/PHD_01_06.png" title="PHD_01_06" class="img-fluid" %}

---



<!-- Responsive 16:9 wrapper -->
<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;border-radius:12px;">
  <iframe
    src="https://www.youtube-nocookie.com/embed/HZcu0jZvc9o?autoplay=1&mute=1&playsinline=1&loop=1&playlist=HZcu0jZvc9o&rel=0&modestbranding=1"
    title="YouTube video"
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;"
    allow="autoplay; encrypted-media; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen
  ></iframe>
</div>

---

# Semidirect Drive Based on Tri-Contacted Plate Harmonic Reducer

Robotic actuators face a performance gap between low-ratio quasi-direct drive (QDD) systems and conventional harmonic drives, which are typically limited to ratios above 30:1. This article presents a tri-contacted plate harmonic reducer (Tri-c PHR) that addresses this challenge by combining axial elastic deformation with a three-point tooth engagement system. The proposed design achieves a 16:1 reduction ratio—a range where conventional harmonic gears face significant design challenges—while maintaining high efficiency and low backlash. An initial prototype validates the design’s feasibility, demonstrating competitive positioning accuracy and backdrivability comparable to commercial harmonic reducers, despite operating at a significantly lower reduction ratio. The Tri-c PHR offers a compelling solution for applications requiring both torque transparency and moderate reduction ratios.

---

<!-- 주석 내용 12 -->

## Tri-Contact Plate Harmonic Reducer for the 10:1–30:1 “Missing Middle” in Robotic Actuation
Robotic actuators sit between low-ratio QDD systems and compact high-reduction harmonic drives, with a practical need for the 10:1–30:1 range to balance torque density, backdrivability, bandwidth, and packaging. However, most commercial harmonic reducers start around 30:1 because lowering the ratio while keeping low backlash typically requires major changes in tooth count and geometry. Other options in this band involve tradeoffs: multistage planetaries increase axial length and mass, cycloidals add sliding losses or larger bearings, and crown-gear/ball reducers can be limited by low engagement or localized contact.

We propose the Tri-Contact Plate Harmonic Reducer (Tri-c PHR) to target this ratio range while maintaining strain-wave characteristics. Tri-c PHR uses three-point tooth engagement instead of the conventional two-point scheme to lower the reduction ratio while distributing load for stiffness and stability. An axial CAM-based wave generator produces axial deformation of a plate-shaped flexspline to achieve multi-tooth engagement, retaining compactness and low backlash. This approach extends the practical reduction range down to about 10:1.



---

<!-- 주석 내용 3 -->

## Axial Plate Deformation for Higher-Efficiency Strain-Wave Transmission
Conventional cup/hat strain-wave gears repeatedly bend a cylindrical flexspline radially, which generates large restoring forces and requires high normal contact loads, increasing friction and reducing efficiency. We use a thin plate-shaped flexspline that deforms axially, driven by a wave generator with axial CAM grooves instead of an elliptical profile. In forward drive, balls in the grooves create axial forces that deform the plate to sustain tooth engagement with the fixed circular spline. In backdrive, torque on the flexspline pushes the balls axially and rotates the wave generator, reducing stress requirements and losses linked to elastic restoration.



---

<!-- 주석 내용 4 -->

## Operating Principle: Ball-Induced Axial Engagement in Plate Harmonics
The figure shows the operating cycle using cross-sectional photographs, where green arrows track a single flexspline tooth. As the wave generator rotates, balls in the CAM grooves induce axial plate deformation and create localized tooth engagement with the circular spline. Over each sequence, the tracked tooth advances by one pitch, generating the reduction motion. This plate-type strain-wave mechanism supports lower reduction ratios than conventional cup/hat designs.



---

<!-- 주석 내용 5 -->

## Why Plate-Type Flexsplines Deform Easier than Hat-Type Harmonics
We model a conventional hat-type flexspline as a thin-walled cylindrical shell that must deform radially at the top rim under 2-point (180°) or 3-point (120°) wave-generator loading, using Donnell–Mushtari–Vlasov thin-shell theory with a Rayleigh–Ritz approach to include membrane and bending effects. Finite-element analysis compares a catalog-equivalent size-17 geometry with matched diameter, 100 teeth, and 0.7 mm tooth height, while using 0.3 mm thickness for the plate design versus 0.15 mm for the hat-type. With axial deformation, the plate-type flexspline reduces radial restoring-force demands, which become pronounced in 3-point loading due to bending stiffness. In FEA, the plate-type requires ~10 N for 0.7 mm deformation, while the hat-type requires ~75 N for 0.35 mm deformation under 3-point loading.



---

<!-- 주석 내용 6 -->

## Three-Point Axial Engagement: The Key to Low-Ratio Plate Harmonics
The reducer consists of a housing, a ball-driven wave generator, a lower ring, a plate flexspline, and a circular spline, with axial CAM grooves phased at 120° to realize tri-contact engagement. During rotation, steel balls in the grooves apply axial forces that deform the plate flexspline and engage the circular spline at three evenly spaced zones. Two-point contact cannot reach low ratios without challenging tooth geometry, while four-point contact lowers per-zone engagement and limits torque capacity. The three-point design shares load over 120° segments and keeps about 25% total tooth engagement, supporting torque transmission with lower deformation force than radial approaches.



---

<!-- 주석 내용 9 11 12 -->

## Prototype Validation: Transparency-Driven Design and Competitive Precision

The left figure summarizes force measurements across transfer angles from 25° to 75°, where the transmission clearly peaks around 35° and aligns with our theoretical prediction. Because this work prioritizes torque transparency for low-ratio actuation, we adopted 35° as the prototype’s optimal transfer angle.

The middle figure reports static positioning performance from 3,733 random target commands, comparing measured output angles against reference values. The Tri-c PHR achieves a 0.631 arcmin mean error and a 5.938 arcmin RMS error (σ = 5.905 arcmin), with a 15.641 arcmin peak error—competitive results for a first prototype operating at 16:1.

The right figure presents the backlash measurement obtained by applying constant torque to the driven motor while fixing the driving motor. The measured backlash is 78.99 arcsec, showing that the tri-contact plate architecture can retain low-backlash behavior even at a substantially lower reduction ratio than conventional harmonic reducers.


---

<!-- 주석 내용 14 -->

## Benchmarking Efficiency Against Commercial Harmonic Drives
As a baseline, we measured the efficiency of SHF-series harmonic reducers (30:1) in sizes 14, 17, and 20 under comparable rated-torque conditions, obtaining 63.61%, 60.78%, and 56.15%. The measured SHF-17 efficiency (60.78%) was slightly higher than the predicted value (58.8%), which can be explained by test-condition differences such as load-point selection and minor environmental variation. Similar factors account for the smaller deviation in SHF-14 and the larger difference in SHF-20. These results indicate the setup is suitable for relative comparison, while small offsets from catalog data are expected.



---

<!-- 주석 내용 15 16 -->

## Torque Transparency and Dynamic Stability in the Tri-c PHR Prototype

The left figure presents the starting-torque tests that quantify static friction in both directions. In the left figure, forward starting torque (with 0 N·m output command) begins motion at 8.5 Ncm, which is comparable to SHF 30:1 size 14 and 17 measured under the same setup (6.1 and 8.41 Ncm). In the left figure, backward starting torque (with 0 N·m input command) reaches 1.91 N·m, showing a brief peak near 0.75 s consistent with elastic snap during tri-contact load redistribution.

The middle figure shows time-domain torque signals under four operating conditions (200/1000 r/min and 1/3 N·m loads). In the middle figure, torque transmission remains steady with small peak-to-peak variations of 0.086–0.171 N·m, corresponding to roughly 3.2–10.6% of the mean torque level. This indicates smooth, repeatable torque delivery even as speed and load increase.

The right figure summarizes the frequency-domain analysis of the same torque data. In the right figure, 200 r/min cases are dominated by a main component around 0.77 Hz with secondary low-frequency content, while 1000 r/min cases spread across multiple components (0.23–3.74 Hz). In the right figure, all vibration amplitudes stay below 0.025 N·m, confirming stable operation across all tested conditions.


---


**Plate Harmonic Reducer with a Profiled Groove Wave Generator**

```bibtex
@inproceedings{You2025Plate,
  author={You, Seungbin and Jung, Jaesug and Sung, Eunho and Park, Jaeheung},
  booktitle={2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
  title={Plate Harmonic Reducer with a Profiled Groove Wave Generator},
  year={2022},
  pages={1900-1907},
  doi={10.1109/IROS47612.2022.9981317}}
}
```

---

**Semidirect Drive Based on Tri-Contacted Plate Harmonic Reducer**

```bibtex
@inproceedings{You2025Plate,
  author={You, Seungbin and Sung, Eunho and Kim, Dongjun and Kim, Juhyun and Park, Jaeheung},
  journal={IEEE/ASME Transactions on Mechatronics}, 
  title={Semidirect Drive Based on Tri-Contacted Plate Harmonic Reducer}, 
  year={2025},
  pages={1-11},
  doi={10.1109/TMECH.2025.3628311}}
}
```
