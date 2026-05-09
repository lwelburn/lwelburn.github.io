---
layout: page
title: Hypersonic Actuator
description: a project that redirects to another website
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
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hypersonic/Design.png" title="BlockDiagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Proposed design of the experimental setup.
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

## Linear Actuator Control



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Hypersonic/BlockDiagram.png" title="BlockDiagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Block diagram for the experimental setup.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
