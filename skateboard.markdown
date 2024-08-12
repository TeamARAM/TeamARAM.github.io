---
title: "Online Planning and Control of Physics-Based Skateboarding Animation"
layout: splash
permalink: "/projects/skateboard"
---

# Online Planning and Control of Physics-Based Skateboarding Animation

_MSc Thesis_

<div style="display: flex; align-items: center;">
<div>
ELIAS MIKKOLA
</div>
<div style="padding-left: 10px; font-size: 18px;">
Aalto University, Finland
</div>
</div>

---

<style>
    div {
        /* border: 1px solid black; */
</style>

<div style="align: center; text-align: center; padding-bottom: 10px;">
<img class="teaser" src="{{'/assets/imgs/skateboard_teaser.gif' | relative_url}}" />
</div>
<div style="text-align: center;">
The front-view (left) and side-view (right) of an example deployment of the planning and control system. The agent is capable of producing pushing motions as well as goal-conditioned steering. 
</div>

## Paper: [AaltoDoc](https://aaltodoc.aalto.fi/items/3d76eb38-cedf-473b-b19f-e6e9d604215b)

This thesis introduces a simulated system for skateboarding, integrating a mechanical approximation of a real-life skateboard into a simulated and simplified skateboard model onto which we apply online planning-based control techniques. Our system design focuses on replicating realistic skateboarding movements, using MuJoCo Model Predictive Control (MJPC) framework and utilizing well-validated implementations of model-based planning algorithms, such as iterative Linear-Quadratic Gaussian with Sampling (iLQS). We incorporate a humanoid model to enact the skateboarding maneuvers, formulating skateboarding as a robotic control task, and delegate the control task to reference pose tracking, where subtasks like pushing and steering are solved with hand-crafted heuristic poses and carefully engineered reward functions without the need for recorded motion capture data. We demonstrate the validity of our approximate skateboard mechanics and our system's performance in replicating the pushing and steering movements. Our experiments with the fundamental Ollie trick demonstrate limited success in going beyond the locomotion on flat terrain. Our quantitative and qualitative analyses offer insights into the trade-offs between task efficiency and robustness and the performance differences across sampling and gradient-based planning algorithms. This work serves as a foundation for future research, providing a baseline and benchmark environment for various forms of assisted locomotion styles and skill sets.

### Summary

We formulate skateboarding as a compound movement involving two distinct phases of motion (pushing and steering). The phase transition is implemented as a simple check of the character's center-of-mass (COM) velocity. Each one of pushing and steering is translated task into a model-based control task with a custom reward function. The system presented applies off-the-shelf reference implementations of state-of-the-art Model Predictive Control (MPC) algorithms paired with MuJoCo physics simulator to solve the control task.

<div style="align: center; text-align: center;">
<div>
<img src="{{'/assets/imgs/skateboard_summary.png' | relative_url }}">
</div>
<div>
An overview of the system with task-switching logic. The state machine has two states for the pushing and steering and a failure state, which terminates the simulation run. 
</div>
</div>

### Citation

<pre style="line-height: 1.4; overflow: auto; font-size: 0.5rem;">
@thesis{mikkola2023online,
  title={Online Planning and Control of Physics-Based Skateboarding Animation},
  author={Mikkola, Elias},
  year={2023},
  school={Aalto University}
}
