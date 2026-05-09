---
layout: page
title: Hypersonic Actuator
description: control of proposed actuators for hypersonic vehicle applications
img: assets/img/Hypersonic/IMG_4952.JPEG
importance: 2
category: research
---

## Piezoelectric Control

**Piezoelectric Stacks**

Piezo stacks use a solid material to convert electrical energy into mechanical energy and can be used for various applications such as actuators, motors, sensors, and energy harvesting devices.

**Advantages:**
- fast response time
- unlimited resolution
- no moving parts or aging
- high efficiency
- produce large forces

**Disadvantages:**
- force production in only one direction
- nonlinearities in modeling due to hysteresis
- temperature effects on position

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hypersonic/BlockDiagram.png" title="BlockDiagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Block diagram for the experimental setup.
</div>

**Feedforward Reference Signal Compensation**
The goal is for the reference signal and the plant output to be equal.
Since the reference signal (disturbance) is known, this error can be limited.
Limitations
Does not compensate for outside disturbances (e.g., temperature/pressure fluctuations).
If the compensator is analog, the hardware (electronic, pneumatic, or hydraulic) cannot replicate the dynamics exactly [9].
If the compensator is digital, the dynamics are limited due to quantization and sampling effects [9].

**Feedforward Disturbance Rejection**
The goal in disturbance rejection is for the plant input signal to be unaffected by the disturbance.
Limitations
The disturbance must be measured accurately and immediately.
This can be difficult to realize physically due to sensor limitations, delays, and various noise.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hypersonic/WithoutComp.png" title="WithoutComp" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hypersonic/WithComp.png" title="WithComp" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Comparison of performance without and with feedforward compensation.
</div>


## Linear Actuator Control





<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <video width="100%" controls class="rounded z-depth-1">
            <source src="/assets/video/Hypersonic/Test.mp4" type="video/mp4">
        </video>
    </div>
</div>
<div class="caption">
    Hardware test.
</div>


