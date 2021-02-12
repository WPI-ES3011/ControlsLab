# Lab 2: Mathematical Modeling I

<!-- ###### Description
* Learn how to develop mathematical models of physical dynamic systems. This would include:
    * Mass-spring-damper
    * DC motor
    * Self-balancing robot

###### What to Submit
* Report showing a summary of exercises completed for MATLAB and Simulink.
    * MATLAB code showing the state-space model of each dynamic systems -->


<!-- ![work_in_progress](../media/wip.jpg) -->

#### Introduction

Welcome to the second session of the ES3011 experimental labs. In this lab, we focus on mathematical modeling. The central question is *"How do describe/model our physical system mathematically to be able to anaylze its behavior?"*

We will cover three sections in this lab:

1. Mathematical modeling of basic dynamical systems

2. Mathematical modeling of of the BalBot (self-balancing robot)

3. Testing Balbot IMU Calibration

##### Learning Outcomes
Our goal at the end of this labs is that you should be able to:

* Understand and describe/model physical dynamic systems mathematically using differential equations
* Convert the differential equations to state-space model form by hand and using MATLAB functionality



*** 
<br>

#### 1. Mathematical Modeling of Basic Dynamical Systems

In this section, you will develop mathematical models for basic dynamical systems considered in control systems such as the mass-spring-damper and the DC motor. These models will then be put into state-space representation which will be used in future lab sessions for simulation and analysis.

##### Instructions:
In this lab [instruction sheet](../documents/Lab2.pdf),

* Review the MATLAB Intro section
* Complete problems I (Mass-spring-damper) and IV (Motor position)

*** 
<br>

#### 2. Mathematical Modeling of the BalBot

![robot](../media/robot.png)

In this section, we will derive the mathematical model for the Balbot.

##### Instructions:
In this lab [instruction sheet](../documents/ES3011_LAB2.pdf),

* You are required to answer all 5 questions in the sheet and record your solutions in your report.

*** 
<br>

#### 3. Testing Balbot IMU Calibration


In Lab 1, we completed the IMU calibration process to ensure the robot get accurate feedback from the IMU sensor about its orientation. In this section, we will now test the calibration process by reading off the robot's pitch values on MATLAB using serial comm.

##### Instructions:

**1. Update your Balbot software:**

- To update the Balbot software on your local PC, please run the `git pull` command in the directory where you cloned the WPI-ES3011 repository
    
<!-- ``` shell
$ git pull
``` -->

**2. Build and upload code to the Balbot:**

- First, connect the robot to your PC via USB.
- Start up VS Code and, following the procedure in Lab 1, build and upload the code to the robot.


**3. Test the IMU calibration on MATLAB:**

- Next step is to start up MATLAB. 
- Make sure you navigate to directory where you have saved the WPI-ES3011 Lab software
- Run the following command in your MATLAB command window (instead of <team-ID> add your actual team ID, e.g. 'Team 1')
``` matlab
>> balbot_serial(<team-ID>)
```

- Make sure you observe that the pitch value changes correctly as you manually move the robot about the X-axis.
- Take screen shots of your MATLAB output (similar to Fig. 2) when the robot is in three positions:
    - Upright position (pitch = ~0 rad)
    - Leaning backward (as far as you can go)
    - Leaning forward (as far as you can go)


<br>

*Fig 1:*
![lab2-command](../media/lab2-command.png)

*Fig 2:*
![lab2-result](../media/lab2-result.png)


*** 
<br>


#### What to Submit:
Prepare a report which contains the following:

* **Introduction:** a few sentences to introduce the topic of the lab
* **Section 1:** Mathematical Modeling of Basic Dynamical Systems (MATLAB)
    * Include free-body diagram and/or equations of motion for the two systems assigned.
    * Publish your MATLAB script with the defined state-space models as a PDF. Follow this [guide](https://www.mathworks.com/help/matlab/matlab_prog/publishing-matlab-code.html) to see how to.
* **Section 2:** Mathematical Modeling of the BalBot 
    * Present your answers to the five questions in your report. Make sure you include a free-body diagram of the robot in your report.
* **Section 3:** Test the IMU calibration on MATLAB
    * Show the three MATLAB screen shots as described above.
* **Conclusion:** a few sentences concluding the report explaining the goals, what you learned, and any other conclusions.



<!-- We can take a simplified approach to the modeling problem by decomposing the BalBot system into sub-components. This is a convenient assumption to simplify the modeling task. The sub-components are: (1) the robot wheels, (2) the motors, (3) robot chassis.  -->

<!-- ###### Preliminaries: Review the equivalent free-body diagram for the complete system

Following the system decomposition, we can draw a simplified representation of the robot as above. We have made a few assumptions:

* The robot moves only in the X-Y plane.
* The robot wheels don't slip, hence we can assume the wheel position is linearly related to the wheel radius and angular displacement.

![complete_system](../media/complete_system.jpg)



###### Question 1: Derive the equations of motion for the robot wheel

We have provided the free-body diagram of the robot wheel below. Your task is to derive the equations of motion for the wheel given the forces and torques acting on the wheel.

!!! note
    * `Fx` and `Fy` are the reaction forces of the robot chassis on the wheel.
    * `theta_wheel` is the angular displacement of the wheel.
    * `N` is the reaction force on the ground.
    * `Ft` is the traction force.
    * `Tm` is the motor torque on the wheel.

![wheel](../media/wheel.jpg)


###### Question 2: Derive the equations of motion for the robot chassis

We have provided the free-body diagram of the robot chassis below. Your task is to derive the equations of motion for the chassis given the forces and torques acting on it.

!!! note
    * `Fx` and `Fy` are the reaction forces of the robot chassis on the wheel.
    * `theta_p` is the angular displacement of the robot chassis in the sagittal plane.
    * `Mr` is the mass of the robot chassis.
    * `Tm` is the motor torque on the wheel.

![chassis](../media/chassis.jpg)


###### Question 3: Derive the relationship between motor torque and voltage, speed, etc.

Finally, you need to derive an equation which relates the torque generated by the motor and the supplied voltage. This is required to replace the torque values in the above equations because the control input to BalBot is motor voltage.

Please refer to the lab [instruction sheet](../documents/Lab2.pdf) for a reminder on the equations describing a DC motor.

![chassis](../media/motor.jpg) -->
