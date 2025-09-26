---
layout: page
title: SNU-Avatar Haptic Glove
description: Novel Modularized Haptic Glove via Trigonometric Series Elastic Actuators
img: assets/img/12.jpg
importance: 1
category: paper
related_publications: false
math: true
---

> We present a **modular haptic glove** for teleoperation. Each finger module (3 potentiometers + 1 servo) provides force feedback via a **Trigonometric Series Elastic Actuator (SEA)**. Although mounted on the **middle phalanx**, we estimate fingertip position using a simple kinematic coupling model. The system was validated during the **ANA Avatar XPRIZE** finals.

---

## Paper Info
- **Title:** SNU-Avatar Haptic Glove: Novel Modularized Haptic Glove via Trigonometric Series Elastic Actuators  
- **Authors:** Eunho Sung, Seungbin You, Seongkyeong Moon, Juhyun Kim, Jaeheung Park  
- **Keywords:** Teleoperation, Haptic Glove, Series Elastic Actuator, Fingertip Estimation, Modular Design
- **Conference:** 2024 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) 


# Motivation

Reliable finger posture capture and safe, informative force feedback are critical for real-world teleoperation. IMU- or vision-based gloves suffer from drift, lighting, or tracking constraints; soft gloves can be comfortable but complicate precise force feedback and maintenance. For the Avatar XPRIZE scenario, we opted for a rigid exoskeletal architecture with active force feedback and robust position sensing.

# Key Contributions
	•	Modular finger unit: 3× potentiometers (AA + FE×2) + 1× servo + spring for pose + force in one module.
	•	Trigonometric SEA: Uses joint geometry to infer tendon length change, enabling force control with fewer encoders.
	•	Middle-phalanx mounting with fingertip estimation: No fingertip sensor—derive fingertip from DIP–PIP coupling and phalange length ratios.
	•	Operator-ready design: Boa system fitting, dovetail plate to haptic arm, Arduino-based I/O, easy add-ons (e.g., vibration).
	•	Validation: Force accuracy tests, fingertip estimation study, and Grasp Taxonomy on the SNU-Avatar hand.

# Hardware at a Glance
	•	Modules: thumb/index/middle/ring = 4 modules on the dorsal frame.
	•	Per module: 5 links / 4 joints; measures MCP-AA (1) and FE (2); final joint is passive for comfort; Velcro middle-phalanx mount.
	•	Size/weight (approx.): unfolded 250×175×130 mm; worn length up to 340 mm; ~500 g including electronics.
	•	Wearing & I/O: Boa tensioning; soft synthetic leather pads; Arduino Mega and serial PC link; extra pins for add-ons.


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
