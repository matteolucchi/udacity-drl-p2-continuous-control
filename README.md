# Project 2: Continuous Control - Udacity DRL Nanodegree
Implementation of a Deep Reinforcement Learning agent to solve the Unity Reacher environment.

This repository contains all the material relative to the implementation of the Project 2 of the [Udacity Deep Reinforcement Learning Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893) program.


## The Environment
The environment consists of a double jointed arms that can move to a target location. The goal of the agent is to maintain the position at the target location for as many time steps as possible. The full environment consists of 20 identical copies of the double jointed arm.  

![continuous_control](https://user-images.githubusercontent.com/36470989/62230382-f90dc500-b3c1-11e9-9692-43c08819c691.gif)

The following description is for a single double-jointed arm.
### State Space
- **Size:** 33

- **Content:** Position, Rotation, Velocity and Angular Velocities of the arm

### Action Space
- **Size**: 4

- **Actions:** Torque to be applied to the joints

### Reward

- **+0.1** : for each step that the agent's hand is in the target location

### Goal

The environment is considered solved when the agent gets an average score of *+30* over 100 consecutive episodes, and over all agents

## Installation

Follow the instructions below to install the software necessary to run the agent in the environment.

**1.** Set up the Python environment on your machine by following the [instructions in the DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies).

**2.** Download the Unity environment:
- [Linux](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
- [Mac OSX](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
- [Windows 32-bit](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
- [Windows 64-bit](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

**3.** Place the unzipped folder just downloaded in the `p2_continuous-control/` folder in the DRLND GitHub repository.

**4.** Clone [this repository](https://github.com/matteolucchi/udacity-drl-p2-continuous-control) in the `p2_continuous-control/` folder in the DRLND GitHub repository.

## How to run the code

The agent can be tested and trained in the [Continuous_Control.ipynp](https://github.com/matteolucchi/udacity-drl-p1-navigation/blob/master/Continuous_Control.ipynb) python notebook. Following the instructions in the notebook it is possible to see our trained agent in action or to train a new agent using the hyperparameters of your choice and to see your agent in action. 
