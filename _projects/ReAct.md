---
layout: page
title: ReAct Hand
description: Bioinspired tendon-driven robotic hand
img: assets/img/ReAct/ReAct.png
importance: 1
category: research
related_publications: false
---

## Motivation
Many industries implement robotic arms for product manufacturing. Most of these arms 
are limited to ≤ 6 DoF, restricting delicate manipulation. Previous research efforts 
have implemented deep reinforcement learning (DRL) on robotic hands, but many lack 
the physical robot to validate their algorithms, or are not bioinspired.

## Design
The **ReAct Hand** (Remote Actuation Hand) is a bioinspired, tendon-driven robotic hand 
designed for dexterous manipulation tasks. Actuators are mounted remotely and transmit 
force through tendons, mimicking the musculotendon architecture of the human hand.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ReAct/ReAct2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Preliminary CAD design of the forearm, wrist, and hand.
</div>

A single finger is modeled and tested to validate the design before implementing the entire hand. Each finger has 4 DoF (RRRR) and is tendon-driven by 8 independent tendons/motors.
<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ReAct/nullConfig.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ReAct/workspace.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Preliminary CAD design of the forearm, wrist, and hand.
</div>

## Demos
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <video width="100%" controls class="rounded z-depth-1">
            <source src="/assets/video/tracking.mp4" type="video/mp4">
        </video>
    </div>
</div>
<div class="caption">
    Point tracking in simulation.
</div>

The challenges of long transmission lines are demonstrated in the video below. PTFE tubes bend and twist under large loads.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <video width="100%" controls class="rounded z-depth-1">
            <source src="/assets/video/flexing.mp4" type="video/mp4">
        </video>
    </div>
</div>
<div class="caption">
    Simple finger movement.
</div>

Given an applied static wrench, the goal is to apply the necessary joint/motor torques to maintain static equilibrium. It is assumed that the mass of each link is negligible and that friction losses are minimal. In the test below, the objective was to push with the required force to measure 300 g on the scale.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <video width="100%" controls class="rounded z-depth-1">
            <source src="/assets/video/scaleTest.mp4" type="video/mp4">
        </video>
    </div>
</div>
<div class="caption">
    Static wrench evaluation.
</div>