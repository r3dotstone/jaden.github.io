---
layout: default
title: Class Projects
permalink: /classprojects/
---

## Here are Some of the Cool Things that I've Done in my Classes

### ECE392: Robotics, Vision, and Control Independent Side
A professor reached out to myself and a fellow integrative engineer (Peter Fabens '24) focussing in robotics because he wants to teach a robotics course in the coming years. We were tasked with reading 
<a href="url">Peter Corke's</a> textbook, Robotics, Vision and Control, and collaborating on exrecises for every chapter to be adapted into labs for the course. Corke's textbook pairs with two freeware libraries: 
<a href="https://github.com/petercorke/robotics-toolbox-matlab">Robotics Toolbox for MATLAB</a> and <a href="https://github.com/petercorke/machinevision-toolbox-matlab">Machine Vision Toolbox for MATLAB</a>. Detailed below are a selection of our demonstrations of critical robotics tools and algorithms, programmed in MATLAB and Simulink.


#### Trajectory Planning
In this example, the task is to navigate the aisles of the grocery store, Giant, with as a quadcopter. This is done by establishing waypoints the quadcopter needs to travel through, planning a multi-segment trajectory that maximizes the quadcopters speed, and passing that to a dynamic model of a quadcotper.

<img src="https://r3dotstone.github.io/portfolio/media/quadGiant.png" height="300" />

 _Orange is the planned path, while the path actually taken by the quadcopter with oscillations and wider turning radii_

[Video coming soon]
<video style="max-height: 300px; width: auto;" controls>
    <source src="https://r3dotstone.github.io/portfolio/media/quadGiantVideo.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video> 

_Live output of the dynamic model_

[Velocities coming soon]

_Velocity vs. Time_

#### Path Planning
In a scenario where a robot needs to find a path from a start point to an end point, it must generate it's own waypoints.

<img src="https://r3dotstone.github.io/portfolio/media/dxformXY.png" width="200" /><img src="https://r3dotstone.github.io/portfolio/media/dxformIso.png" width="200" />

_Distance transform using an occupancy grid_


<img src="https://r3dotstone.github.io/portfolio/media/undilatedMap.png" height="200" /><img src="https://r3dotstone.github.io/portfolio/media/dilatedMap.png" height="200" />


_Map dilation_

<img src="https://r3dotstone.github.io/portfolio/media/quadDstar.png" height="300" />

_Planning with D* using an occupancy grid_

#### Kalman Filter
Below is an example using the scenario of an autonomous vehicle driving along a road, undergoing a lane change. It periodically sees lane markers on the road and uses them as landmarks to update it's position estimate.

<img src="https://r3dotstone.github.io/portfolio/media/unfilteredPositionKalman.png" height="300" />

_Estimated position using just odometry, no Kalman filter_

<img src="https://r3dotstone.github.io/portfolio/media/filteredPositionKalman.png" height="300" />

_Estimated position using Kalman filter_

<img src="https://r3dotstone.github.io/portfolio/media/errorUncertaintyKalman.png" height="300" />

_Estimated error and uncertainty over time_

#### Range Finder Mapping
Without a map provided to a robot, it must use it's sensors to estimate the position of it's surroundings. Simulated below is a mobile robot modeled as a "unicycle". It is equipped with a laser range finder. All sensors on the robot are simulated with gaussian noise and a diagonal covariance.

<video style="max-height: 300px; width: auto;" controls>
    <source src="https://r3dotstone.github.io/portfolio/media/romiMapping.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>


### ES302: Robotics Systems and Design
This course was gave us a broad understanding of the different ways to control a robot. It focussed on real hardware and software integration, meaning that we also learned how to rigosously troubleshoot eratic platforms. Schemes that we implemented include: 
- procedural control
- finite state machines
- transformation and rotation matrices
- odometry
- quaternions
- forward and inverse kinematics
- the Jacobian and joint/configuration space
- wrench and twist
- proportional control
- Dijkstra's algorithm
- computer vision and convolution
- basic simultaneous localization and mapping 

#### Using a finite state machine to create a lemming robot

<video style="max-height: 300px; width: auto;" controls>
    <source src="https://r3dotstone.github.io/portfolio/media/ES302_A04_2_comped1.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video> 

#### Dijkstra's Algorithm

<video style="max-height: 300px; width: auto;" controls>
    <source src="https://r3dotstone.github.io/portfolio/media/dijkstras.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

#### Inverse Kinematics

<video style="max-height: 300px; width: auto;" controls>
    <source src="https://r3dotstone.github.io/portfolio/media/invKin.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

#### Final Project: Simulating a User-Demand Blended Power Hybrid

A parallel course of study during the course was the developement of a research project following the rigorous academic process. We conducted developed search protocol, conducted literature screening, and wrote a literature review of the existing research in the field our proposed final project published on IEEE Xplore. We concluded the semester by tackling our projects either in simulation or physical realization, writing a comprehensive resarch article, and creating a project poster to be presented alongside senior design projects.

My project was to assess the feasability of a parallel blended power compensation (PBPC). This means that I build a simulation of a hybrid car that mixes power directly from an ICE and electric motor such that the electric motor contributes enough power to bring the total power up to an ideal quantity that varies with RPM and throttle position. Please see the poster and video below for more details.

<object style="height: 450px; width: 600px;" data="https://r3dotstone.github.io/portfolio/media/ES302_Stone_FinalPoster.pdf" type="application/pdf" >
    <embed src="https://r3dotstone.github.io/portfolio/media/ES302_Stone_FinalPoster.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://r3dotstone.github.io/portfolio/media/ES302_Stone_FinalPoster.pdf">Download PDF</a>.</p>
    </embed>
</object>

<video style="max-height: 300px; width: auto;" controls>
    <source src="https://r3dotstone.github.io/portfolio/media/G__.shortcut-targets-by-id_1_PeZcmc5YVnmj6_6Aui8IlOqeOcDBKTt_ES302_Stone_FinalProject_WeBots_worlds_highwayOvertake_mod.wbt (FinalProject_WeBots) - Webots R2022a 2023-02-24 10-25-02.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

### ECE 322: Introduction to Solid State Devices and Circuits

In this class we learned how to both analyze and design circuits constructed of low-level solid state components including op-amps, diodes, and transistors. For our final project we were tasked in pairs to design transmitter and reciever circuits to transform audio signals to optical ones and back. Below are snippets of work from that project.

<img src="https://r3dotstone.github.io/portfolio/media/SPICE1.png" width="200" /> <img src="https://r3dotstone.github.io/portfolio/media/SPICE2.png" width="200" />

_Spice for the Main Circuit and Test Bench_

<img src="https://r3dotstone.github.io/portfolio/media/CIRC1.jpg" height="300" /> <img src="https://r3dotstone.github.io/portfolio/media/CIRC2.jpeg" height="300" />

_Components Soldered on a Custom Prototype Board_ 

### CE181: Cities

I took this course while studying abroad in Bonn, Germany. It gave us crucial insight into the engineering and it's societal effects within urban areas. I researched and analyzed zoning's effect on people throughout different cities that I visited while in Europe. Below is the presentation, but you can read the full paper <a href= "https://r3dotstone.github.io/portfolio/media/CitiesFinalPaperFD_04.29.pdf" target="_blank"> here </a>.

<object style="height: 450px; width: 600px;" data="https://r3dotstone.github.io/portfolio/media/CitiesFinalPresentation.pdf" type="application/pdf" >
    <embed src="https://r3dotstone.github.io/portfolio/media/CitiesFinalPresentation.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://r3dotstone.github.io/portfolio/media/CitiesFinalPresentation.pdf"> Download PDF</a>.</p>
    </embed>
</object>

### EGRS251: Introduction to Public Policy

This class is crucial to the integrative engineering major, giving us a framework to understand engineering in the context of government and society. We learned and modeled the policy-making process, analyzing how engineering interacts with it. I examined the policy landscape surrounding the right to repair, using my technical knowledge to inform my analysis and recommendations.

<object style="height: 450px; width: 600px;" data="https://r3dotstone.github.io/portfolio/media/PolicyPresentation.pdf" type="application/pdf" >
    <embed src="https://r3dotstone.github.io/portfolio/media/PolicyPresentation.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://r3dotstone.github.io/portfolio/media/PolicyPresentation.pdf"> Download PDF</a>.</p>
    </embed>
</object>

<object style="height: 800px; width: 600px;" data="https://r3dotstone.github.io/portfolio/media/PolicyBrief.pdf" type="application/pdf" >
    <embed src="https://r3dotstone.github.io/portfolio/media/PolicyBrief.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://r3dotstone.github.io/portfolio/media/PolicyBrief.pdf"> Download PDF</a>.</p>
    </embed>
</object>
