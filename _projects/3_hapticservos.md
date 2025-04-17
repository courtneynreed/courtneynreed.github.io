---
layout: page
title: haptic servos
description: self-contained vibrotactile rendering system for creating material experiences
img: assets/img/proj_preview/hapticservo.jpg
importance: 1
category: designs
related_publications: Reed_TEI22_Vibrotouch, Sabnis_CHI23_HapticServos, Sabnis_CHI23_TactileSymbols
---

{% if site.data.repository-hapticservo.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repository-hapticservo.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}

<br>
Haptic Servos are fully open source and [all code, examples, and information on getting setup with Teensyduino (based on Arduino IDE) and PlatformIO can be found on Github.](https://github.com/sensint/Servo_Haptics)

There is also a compatible [Haptic Material Designer](https://github.com/sensint/Haptic_Material_Designer) created by Gabriela Vega, Nihar Sabnis, Dennis Wittchen, and Paul Strohmeier. The Designer uses a desktop-based GUI for creating material experiences with Haptic Servos. <br><br>

<div class="row">
    <div class="col-sm mt-4 mt-md-0">
        {% include figure.html path="assets/img/proj-hapticservos/servo.png" title="" class="img-fluid rounded" %}
        {% include figure.html path="assets/img/proj-hapticservos/b-tuis.png" title="" class="img-fluid rounded" %}
    </div>
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/proj-hapticservos/a-tuis.png" title="" class="img-fluid rounded" %}
    </div>
</div>
<div class="caption">
    PCB versions of the VoxEMG. The v3.1 eTextile Configuration (left) features castellated inputs for conductive thread input and loops for textile integration. The v3.1.2 Bela Mini Capelet (middle, right) slots directly into the A0 and A1 analogue inputs, power, and ground from the Bela Mini.
</div>

## about

Haptic Servos were designed by the [Sensorimotor Interaction Group (senSInt)](https://sensint.mpi-inf.mpg.de/) at the [Max Planck Institute for Informatics (MPI-INF)](https://www.mpi-inf.mpg.de/home). The main contributors are Paul Strohmeier, Nihar Sabnis, Dennis Wittchen, Valentin Martinez-Missir, and myself. The designs encapsulate all timing-sensitive elements and hardware setup to create a rich variety of material experiences. Research work, primarily undertaken by Nihar in his PhD research, explores how Haptic Servos can be used to render continuous and dynamic, motion-coupled material experiences in tangible user interfaces.<br>

Haptic Servos enable rapid rendering of diverse material experiences in a plug-and-play sensor-actuator path. The open source Haptic Servo shield is compatible with the Arduino IDE/[Teensyduino](https://www.pjrc.com/teensy/teensyduino.html) and [PlatformIO](https://platformio.org/). The firmware has been tested for both the Teensy 3.5 and Teensy 4.1 microcontrollers.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/proj-hapticservos/workflow.png" title="" class="img-fluid rounded" %}
    </div>
</div>
<div class="caption">
    The Haptic Servo signal flow diagram between analogue sensor, control device/microcontroller, and actuator.
</div>

## related publications:
