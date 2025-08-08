# PyBullet-Based Pick-and-Place Pipeline with Franka Panda

This repository presents a simulation framework for executing multi-object pick-and-place tasks using the Franka Emika Panda robot arm in PyBullet. It was developed for experimental robotics research and is designed to be extensible for manipulation, motion planning, and learning-based control tasks.

---

## Overview

The main script (`6_advanced_pick_and_place.py`) performs the following operations in a physics simulation:

- Loads a static workspace with ground and table
- Spawns multiple small cubes at randomized positions
- Computes inverse kinematics (IK) for reaching grasp targets
- Interpolates joint trajectories for smooth motion
- Executes grasp, lift, and place actions
- Evaluates success for each pick-and-place operation
- Logs structured results for downstream analysis

---

## Features

-  Object-agnostic grasping logic (parameterized URDF)
-  Inverse kinematics-based trajectory generation
-  Smooth joint-space interpolation
-  Gripper actuation with force control
-  Automatic success validation
-  Logging to `.json` for reproducibility

---

## Environment Setup

### Requirements

Python 3.7+

Install dependencies:

```bash
pip install pybullet numpy
