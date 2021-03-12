# LAB 6: Stability Analysis, Frequency Response & Complete Controller Design



<!-- ### Description:
* Learn how to analyze stability and frequency responses with Bode plots for the self-balancing robot
* Learn how to reduce steady-state error 
* Learn how to create a lag compensator

### What to Submit:
* Report showing a summary of exercises completed by hand as well as with MATLAB.
 -->

#### Introduction

Welcome to the sixth session of the ES3011 experimental labs. 

In this lab, you will learn how to analyze stability and frequency responses with bode plots. Also, you will learn how to reduce steady-state error and learn how to create a lag compensator.

We will cover three sections in this lab:

1. Stability analysis and frequency response.
2. Complete controller design for the BalBot (self-balancing robot).

##### Learning Outcomes
Our goal at the end of this labs is that you should be able to:

* Understand how to analyze stability and frequency response.
* Understand how to design complete controllers for real robotic systems (the BalBot) using state feedback and PID controller.

***
<br>

#### 1. Stability Analysis and Frequency Response

In this section, you will analyze stability and frequency responses. Bode diagram will be plotted.

##### Instructions:
In this lab [instruction sheet](../documents/Lab6.pdf),

* Complete the MATLAB section (problems I, cruise-control car).

*** 
<br>

#### 2. Complete Control Design for the BalBot (self-balancing robot)

![robot](../media/robot.png)

In this section, we will design a complete controller for the robot.

##### Instructions:

1. Build and run the simulation firstly. Please follow this lab [instruction sheet](../documents/ES3011_LAB6.pdf). Answer all the questions in the report.


Hint: You can learn about the main idea of how to simplify the system, this is for state feedback controller: [instruction sheet](../documents/Hint_Lab6.pdf).


2. **Implementing on the Balbot**

    Once we have a good feedback controller in simulation, we can then implement it on the physical balbot.

    - Update the Balbot software on your local PC by running the `git pull` command in the directory where you cloned the WPI-ES3011 repository.

    - Insert your **PID gain** values (**model parameters** and **state feedback gain** values have been inserted in Lab 5) in the controller.cpp file. You will see the points marked in the file.

    - Load the code to the robot and observe its behavior. 
        - Hint: The behavior of the balbot in balancing would be based on the poles you defined above and the resulting gains. If you find unsatisfactory behavior, modify your pole values and update the gains.

    - Take a very short video (convert to a short GIF) of your best performing controller and **report** what control parameters are. See below for reference.

    Hint: The gif should be like that you push (smoothly) the robot at the left/right edge, and then the robot can recover from the sudden impact.

***
<br>

#### What to Submit:
Prepare a report which contains the following:

* **Introduction:** a few sentences to introduce the topic of the lab
* **Section 1:** Stability and Frequency Responses
    * Include plots and comments as the questions request.
* **Section 2:** Complete Control Design for the BalBot (self-balancing robot)
    * Make sure you include all the plots, equations and observation discussions requested above.
    * Upload the short GIF of your robot balancing after you push it (as you see in the figure above) to Canvas. Follow [link](https://ezgif.com/video-to-gif) for a good GIF creator.
* **Conclusion:** a few sentences concluding the report explaining the goals, what you learned, and any other conclusions.





