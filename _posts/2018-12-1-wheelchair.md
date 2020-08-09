---
layout: post
title: "All-terrain Wheelchair"
featured-img: wheelchair_banner
categories: [Mechanical, Electrical, Design]
---

For my mechanical engineering senior design project, I worked on a team of 7 people to build an all-terrain wheelchair. We started this project from scratch and worked on it for one semester with the goal of creating a wheelchair a local resident could use in sand and forest terrains. I was in charge of all electrical systems and welding of all mechanical components. After one semester, we successfully created a working wheelchair that could be used in the sand.

[Read the full report (pdf)](files/ME450_F18_FinalReport_7.pdf)

My primary role on the team was the high voltage accumulator and low voltage controls system lead. I had the most experience with electronics and designed an electrical system capable of powering and controlling four 800W electric motors for our powertrain. The biggest challenges with building my design was time and budget. I only had one semester to complete this project and a shoestring budget, but I successfully built a working electrical system within the time constraint for only $382.

![Wiring Diagram](/assets/img/posts/wheelchair/wheelchairdiagram.jpg)

<div class = "row">
    <div class = "col-12 col-md-6">
        <p>The high voltage accumulator consists of 2 parallel sets of 16 series LiFePO4 3.2V cells (16s2p) to create a 48V 40AH battery. The batteries came as a donation but the supporting battery management systems, plastic insulating box, and charger were purchased. I had very little experience with working with batteries before this project and learned a lot about how to wire them properly.</p>
    </div>

    <div class = "col-12 col-md-6">
        <img src = "/assets/img/posts/wheelchair/batterybox.jpg" alt="Battery Box">
    </div>
</div>

<div class = "row">
    <div class = "col-12 col-md-6">
        <p>The main controller is an Arduino Mega which sends PWM signals (converted to analog via a low pass filter) to e-bike motor controllers. These motor controllers than control the speed of each brushless DC motor in each wheel. NPN transistors controlled by the Arduino simulate physical switches across the motor controller to switch the motor direction. An Arduino Mega was selected over different microcontrollers due to the high number of hardware interrupts which are needed to read the hall sensors in each motor and measure speed. I also wrote all the supporting code to operate the controls system and incorporated dynamic torque vectoring to steer the wheelchair.</p>
    </div> 
    
    <div class = "col-12 col-md-6">
        <img src = "/assets/img/posts/wheelchair/controlsbox.jpg" alt="Arduino Controller">
    </div> 
</div>

<div class = "row">
    <div class = "col-12 col-md-6">
        <p>The wheelchair has a tubular steel spaceframe and an independent trailing link suspension system, also made of 1.00" OD steel tube. I am a very experienced TIG welder thanks to my time on the Michigan Hybrid Racing team and I TIG welded every steel part on our wheelchair. This included the chassis, tabs, and the four suspension control arms.</p>
    </div>

    <div class = "col-12 col-md-6">
        <img src = "/assets/img/posts/wheelchair/wheelchairweld.jpg" alt="Welding the wheelchair">
    </div>
</div>

![Wheelchair in the sand](/assets/img/posts/wheelchair/sandview.jpg)
