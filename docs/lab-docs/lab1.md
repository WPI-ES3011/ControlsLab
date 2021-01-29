# LAB 1: Intro to MATLAB & Self-Balancing Robot Setup

<!-- ### Description:
* Get familiar with basic use of MATLAB and Simulink.
* Set up the environment to program the self-balancing robot on your PC
    * Follow the instructions

### What to Submit:
* Report showing a summary of exercises completed for MATLAB and Simulink.
* Check-out that your robot is set up and operational from your PC. -->

#### Introduction

Welcome to the first session of the ES3011 experimental labs. We have two (2) sections in this lab:

1. Introduction to MATLAB

2. Self-Balancing Robot Setup

##### Learning Outcomes
Our goal at the end of this labs is that you should be able to:

* Perform basic linear algebra computations using MATLAB command window
* Write and run a MATLAB script
* Use the plot function in MATLAB 
* Use basic control system functions such as `tf`, `ss` in MATLAB

<br>

*** 

#### 1. Introduction to MATLAB

In this section, you will get a gentle introduction to MATLAB and how to use it for control systems design and analysis.

##### Instructions:
1. If you don't have MATLAB, please follow this [guide](../documents/HowToDownloadMatlab.pdf) on installing MATLAB.
2. Access the MATLAB Tutorials [here](https://canvas.wpi.edu/courses/23468/files/3430459?wrap=1)
3. Read through the following chapters to get the basics:
    * Chapter 1
    * Chapter 2
    * Chapter 3 (through Identity Matrix, but skip 3D plotting, multi-dimensional arrays and structures)
4. Open up the MATLAB software. Create a MATLAB script that does the following:
    * **Q1:** Add two 3x3 identity matrices and multiplies that result by the vector `[1;2;3]`
    * **Q2:** Plot the function `y = sin(t)` from 0 to 10 seconds with labeled axes and a suitable title.
    * **Q3:** Find the roots of `s^4 + 3s^3 - 15s^2 - 2s + 9`. Hint: First declare `s = tf('s')` and use `zero(_yourFunction_)` to find the roots.

<br>

*** 

#### 2. Self-Balancing Robot Setup

In this section, you will walk through the process of setting up the self-balancing robot and enable your programming environment in MATLAB.

![robot](../media/robot.png)

##### Instructions:
1. If you don't have MATLAB, please follow this [guide](../documents/HowToDownloadMatlab.pdf) on installing MATLAB.
2. Download and set up Visual Studio Code following this [guide](../documents/HowtoDownloadVisualStudioCode.pdf).
3. Download Git (with Git Bash) [here](https://git-scm.com/downloads)
4. Calibrating the robot sensors (on-board IMU):
    * The self-balancing robot uses an IMU (inertial measurement unit) for pose measurement. This sensor needs to be calibrated properly.
    * Follow the instructions [here](../documents/BalBotCalibration.pdf)

<br>

*** 

#### What to Submit:
Prepare a report which contains the following:

* **Introduction:** a few sentences to introduce the topic of the lab
* **Section 1:** MATLAB
    * Publish your script (and its output) as a PDF from MATLAB. Follow this [guide](https://www.mathworks.com/help/matlab/matlab_prog/publishing-matlab-code.html) to see how to.
* **Section 2:** Self-balancing Robot Setup 
    * [*Nothing to report here. Just ensure you are able to calibrate your robot*]
* **Conclusion:** a few sentences concluding the report explaining the goals, what you learned, and any other conclusions.