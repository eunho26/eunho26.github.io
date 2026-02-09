---
layout: page
title: SNU-Avatar Haptic Glove
description: Novel Modularized Haptic Glove via Trigonometric Series Elastic Actuators
img: assets/img/Hapticglove.jpg
importance: 2
category: paper
related_publications: false
math: true
---

> We present a **modular haptic glove** for teleoperation. Each finger module (3 potentiometers + 1 servo) provides force feedback via a **Trigonometric Series Elastic Actuator (SEA)**. Although mounted on the **middle phalanx**, we estimate fingertip position using a simple kinematic coupling model. The system was validated during the **ANA Avatar XPRIZE** finals.

---

# Abstract
The avatar robot is a robot capable of realistic remote operation. In remote operation, the controllability of the glove is crucial. This glove can manipulate the hand interacting directly with the environment at the remote site. The glove must be able to accurately estimate the hand posture and provide haptic feedback to convey information about the remote environment and enhance operability. Throughout the process, user discomfort should be minimized. To achieve this goal, the research proposes providing force feedback to the fingers using Trigonometric Series Elastic Actuators. Haptic gloves are attached to the Middle Phalanx to facilitate the easy installation of additional add-ons, ensuring users feel securely fixed when attached. Additionally, by proposing an algorithm to estimate the fingertip position without directly attaching it to the fingertip, the haptic glove estimates hand posture and delivers appropriate force as needed. Finally, the system, including the haptic glove, participated in the ANA Avatar XPRIZE competition. The avatar system performed eight missions, which included not only remote manipulation of objects but also social interactions, demonstrating its effectiveness.

---

<!-- Responsive 16:9 wrapper -->
<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;border-radius:12px;">
  <iframe
    src="https://www.youtube-nocookie.com/embed/tGXdiD0JgZ8?autoplay=1&mute=1&playsinline=1&loop=1&playlist=tGXdiD0JgZ8&rel=0&modestbranding=1"
    title="YouTube video"
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;"
    allow="autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen
  ></iframe>
</div>

---

# Paper Info

- **Title:** SNU-Avatar Haptic Glove: Novel Modularized Haptic Glove via Trigonometric Series Elastic Actuators
- **Authors:** Eunho Sung, Seungbin You, Seongkyeong Moon, Juhyun Kim, Jaeheung Park
- **Keywords:** Teleoperation, Haptic Glove, Series Elastic Actuator, Fingertip Estimation, Modular Design
- **Conference:** 2024 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)

# Motivation

Reliable finger posture capture and safe, informative force feedback are critical for real-world teleoperation. IMU- or vision-based gloves suffer from drift, lighting, or tracking constraints; soft gloves can be comfortable but complicate precise force feedback and maintenance. For the Avatar XPRIZE scenario, we opted for a rigid exoskeletal architecture with active force feedback and robust position sensing.

# Key Contributions

- Modular finger unit: 3× potentiometers (AA + FE×2) + 1× servo + spring for pose + force in one module.
- Trigonometric SEA: Uses joint geometry to infer tendon length change, enabling force control with fewer encoders.
- Middle-phalanx mounting with fingertip estimation: No fingertip sensor—derive fingertip from DIP–PIP coupling and phalange length ratios.
- Operator-ready design: Boa system fitting, dovetail plate to haptic arm, Arduino-based I/O, easy add-ons (e.g., vibration).
- Validation: Force accuracy tests, fingertip estimation study, and Grasp Taxonomy on the SNU-Avatar hand.

# Hardware at a Glance

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_01_01.png" title="Glove 01-01" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_01_02.png" title="Glove 01-02" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- Modules: thumb/index/middle/ring = 4 modules on the dorsal frame.
- Per module: 5 links / 4 joints; measures MCP-AA (1) and FE (2); final joint is passive for comfort; Velcro middle-phalanx mount.
- Size/weight (approx.): unfolded 250×175×130 mm; worn length up to 340 mm; ~500 g including electronics.
- Wearing & I/O: Boa tensioning; soft synthetic leather pads; Arduino Mega and serial PC link; extra pins for add-ons.



# Working Mechanism

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_02_01.png" title="Glove 02-01" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_02_02.png" title="Glove 02-02" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Trigonometric SEA (Force Feedback)

- Tendon length $s$ for joint angle $\phi$:

$$
s = \sqrt{d^2 + l^2 - 2dl \cos \phi}
$$

- Required motor compensation for a joint change $\phi_1 \to \phi_2$ (pulley radius $r$):

$$
\Delta q = \frac{\sqrt{d^2+l^2-2dl\cos\phi_2} - \sqrt{d^2+l^2-2dl\cos\phi_1}}{r}
$$

- Motor angle for desired force $F$ (spring $k$, geometry $l, l_2, \alpha, \theta_3$):

$$
q = \frac{\left(\sqrt{d^2+l^2-2dl\cos\phi_2} - s_0 - \frac{F l_2 \sin \theta_3}{k l \sin \alpha}\right)}{r} + q_0
$$



#Takeaway:

Output-side potentiometer + geometry ⇒ force without extra encoders on the tendon side.

Fingertip Position Estimation (Middle-Phalanx Mount)

Assumptions often used in hand models:

- Relation between joints: $\theta_{\mathrm{DIP}} = \tfrac{2}{3}\,\theta_{\mathrm{PIP}}$
- Length ratio: $L_p : L_m : L_d \approx 0.50 : 0.30 : 0.20$

<div class="row">
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_01.png" title="Glove_03_01" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_02.png" title="Glove_03_02" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_03.png" title="Glove_03_03" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_04.png" title="Glove_03_04" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

###Grasping with the Tele-Operating Hand

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_05.png" title="Glove_03_05" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


**BibTeX**

```bibtex
@inproceedings{Sung2025SNUAvatarGlove,
  author={Sung, Eunho and You, Seungbin and Moon, Seongkyeong and Kim, Juhyun and Park, Jaeheung},
  booktitle={2024 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
  title={SNU-Avatar Haptic Glove: Novel Modularized Haptic Glove via Trigonometric Series Elastic Actuators},
  year={2024},
  pages={3573-3580},
  doi={10.1109/IROS58592.2024.10802590}
}
```
