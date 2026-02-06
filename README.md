# Graduation Projects (GP1 & GP2)

This repository is dedicated to covering the main lines of work done in graduation projects **GP1** and **GP2**, with some visual aids and results shown in my parts of the presentations of the two projects.

I design my presentations in a minimalistic style with few headings and points to help me remember, organize my speech, and not cause any distractions to the audience, so this README will be more descriptive.

Both projects are implemented in **MATLAB scripts**.

## GP1: Kinematics of Double Wishbone Suspension and Its Visualization

<p align="center">
  <img src="https://raw.githubusercontent.com/semojaw/IntegratedVehicleModelDocumentation/refs/heads/main/IntegratedVehicleModelImages/susWheelRack.png" width="40%">
</p>

1. Developed a function that generates the hard points of suspension and steering geometry (mounts on chassis, link connections, main points like wheel center and contact patch) from some design parameters (anti-dive and anti-squat percentage, C.G. height, swing arm lengths in front and side views, etc.).

2. 3D plotting of the hard points with connecting lines to visualize the design of suspension and steering geometry for all wheels.

3. Implemented a mathematical model to solve the configuration of the system given the inputs:  
   a. Lower control arm angle (φ)  
   b. Steering rack displacement  
   c. Structure of the hard points  
   d. Vehicle general displacement and rotation matrix (optional)  

   The outputs:  
   a. The new position of all hard points  
   b. The new system parameters (wheel/suspension angles, unit vectors, mechanical ratios, etc.)

4. Implemented some 3D definitions for roll centers and pitch centers.

5. Verified the model results with **ADAMS** software.

6. Made a function to link some simple full-vehicle dynamics model data with respective wheel orientations from the kinematic model to visualize them in a Python-based video representation.

<p align="center">
  <img src="https://raw.githubusercontent.com/semojaw/IntegratedVehicleModelDocumentation/refs/heads/main/IntegratedVehicleModelImages/videoScreenshot.png" width="40%">
</p>

## GP2: Development of AMT Control System

1. Modeling and estimating the parameters of a manual transmission test rig, including:  
   a. Simple induction motor  
   b. Clutch nonlinear model with smooth friction model  
   c. Configuring body equations in engagement and disengagement cases with different gear ratios used  
   d. Modeling shifting actuators and clutch actuator with their forces and loads  

2. Designing shifting algorithm and logic.

3. Tuned PID control for actuators.

<p align="center">
  <img src="https://raw.githubusercontent.com/semojaw/IntegratedVehicleModelDocumentation/refs/heads/main/IntegratedVehicleModelImages/fullGearRange.jpg" width="80%">
</p>

4. Modeled discrete MPC for clutch actuator.

<p align="center">
  <img src="https://raw.githubusercontent.com/semojaw/IntegratedVehicleModelDocumentation/refs/heads/main/IntegratedVehicleModelImages/ClutchMPC.jpg" width="60%">
</p>
