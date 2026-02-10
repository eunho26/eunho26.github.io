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

# Advanced Modular Haptic Glove for Precision Teleoperation

Our innovative modular haptic glove features a high-precision 5-link, 4-joint structure designed to capture intricate finger postures while providing realistic force feedback via position control actuators. Engineered for seamless integration with the SNU-Avatar Robot Hand, the 500g lightweight frame utilizes an Arduino Mega and high-precision potentiometers to track complex movements like abduction and flexion with clinical accuracy. For maximum user comfort, the system incorporates the adjustable Boa Fit System and soft synthetic leather, offering an ergonomic, high-fidelity interface that bridges the gap between human intent and robotic execution.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_01_01.png" title="Glove 01-01" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_01_02.png" title="Glove 01-02" class="img-fluid" %}
    </div>
</div>

---
# Advanced Force Feedback and Fingertip Estimation for Remote Manipulation

The designed haptic glove serves as a sophisticated interface that estimates complex finger postures to precisely control remote robotic hands while delivering realistic haptic feedback through a single-actuator system. Utilizing a mechanism similar to Series Elastic Actuators (SEAs), the device measures the deformation of an elastic element via a potentiometer at the second joint, effectively reducing the need for multiple encoders through advanced computational modeling. To provide space for custom fingertip add-ons, the glove securely couples with the user's middle phalanxes, employing a specialized algorithm to accurately estimate fingertip positioning. This integrated approach ensures a high-fidelity telepresence experience, combining hardware efficiency with the flexibility to incorporate additional functional modules at the fingertips.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_02_01.png" title="Glove 02-01" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_02_02.png" title="Glove 02-02" class="img-fluid" %}
    </div>
</div>

---


<div class="row">
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_01.png" title="Glove_03_01" class="img-fluid" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_02.png" title="Glove_03_02" class="img-fluid" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_03.png" title="Glove_03_03" class="img-fluid" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_04.png" title="Glove_03_04" class="img-fluid" %}
    </div>
</div>

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



### Grasping with the Tele-Operating Robot Hand

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Glove_03_05.png" title="Glove_03_05" class="img-fluid" %}
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
