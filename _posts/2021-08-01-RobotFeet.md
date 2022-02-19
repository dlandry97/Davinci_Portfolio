---
title: Humanoid Robot Feet
layout: post
post-image: "/Davinci_Portfolio/assets/IHMC/2021_Nadia_JumpCollage.jpg"
description: This project involves the research and design of feet for the NADIA robot, a hydraulic powered humanoid robot in development at The Institute for Human and Machine Cognition (IHMC).
tags:
- Robotics
- Engineering
- Design
- Research
- IHMC
---

This project started as a literature review of robotic feet for bipedal humanoid robots. There was also extensive research in what type of sensor would be ideal for robot feet considering COP and ground sensing. The findings of the literature review and sensor research were used to design many novel prototype feet that were considered for the NADIA robot. This led to the specification, commision, and testing of a 6-axis force/torque sensor. The testing and implementation of the foot sensor continued throughout my time at the IHMC.



**Literature Review**
The literature review was focused on dynamic robot feet both actuated and passive with the goal to increase efficiency and ability for robotic bipedal locomotion. This review covered humanoid robots from all over the world including Atlas, ASIMO, HRP, LOLA, Sarcos, TORO, Cassie, Digit, WABIAN, and many more. 
My studies showed that having an additional toe linkage would result in a more human-like walking gate and more efficient force transfer throughout locomotion. With toes, the robot would perform a more natural toe-off and heel strike action that improved efficiency by reducing the maximum torque required for forward movement. The toe-off/heel-strike gate also improves efficiency by reducing the lateral movement range of the torso during locomotion, leading to more consistent force and power requirements. 
The addition of toes would also create a more efficient "roll-over shape" which would improve the efficiency for dynamic walking. 


**Sensor**
Robotic foot sensors need to be able to sense the center of pressure from the foot to the ground. To do this, you need to be able to sense 3 axis of force; x-moment, y-moment, z-axial. I decided to move forward with a 6-axis force/torque sensor that measures all moment torques and all axial forces.

I conducted a variety of tests on the 6-axis F/T sensor, including force measurement resolution, historesis testing, thermal drift testing, and long term measurement drift. 

**Photo of load testing setup**
![F/T test setup](/Davinci_Portfolio/assets/IHMC/test_setup.jpg)

Test results led to the discovery of inaccurate measurements due to sensor housing deformation between the mounting holes. To mitigate this, I conducted FEA and physical tests on adapter components that would attach to the deforming surfaces to translate the forces through a structure that would spread the forces evenly between each mounting holes, eliminating housing deformation. Different designs were tested in an attempt to reduce added height and weight. 

**Photos of F/T sensor adaptor FEA**
![adapter FEA1](/Davinci_Portfolio/assets/IHMC/FEA1.png)
![adapter FEA2](/Davinci_Portfolio/assets/IHMC/FEA2.png)
![adapter FEA3](/Davinci_Portfolio/assets/IHMC/FEA3.png)
![adapter FEA4](/Davinci_Portfolio/assets/IHMC/FEA4.png)

**Design and Prototyping**
My initial foot designs included toe linkages that would bring the added benefits to the robot gate. I made these designs with the current sensor structure in mind and was able to print plastic prototypes to demonstrate the movement of the toes. 

**CAD model of the foot with toes**
![cad foot](/Davinci_Portfolio/assets/IHMC/cad_foot.png)

**3D printed model of the foot with toes**
![plastic foot](/Davinci_Portfolio/assets/IHMC/plastic_foot.jpg)

With the limited literature and implementation of toes on robots, the final decision was to not add toes to the NADIA robot foot. Adding the toe linkage would increase the degree of freedom of the robot and add a large amount of complexity to the control system. The developed robot balance and locomotion control system was also not designed to perform with a natural human gate and would need a large amount of redevelopment to implement. The toes would also require strong actuators, which would be large and heavy, increasing the inertial load to swing the leg forward. At the current development of the robot, adding toes would add much more complexity that outweighed the benefits of a human-like toe-off/heel-strike gate.

**Photo of implemented F/T sensor on flat foot**
![foot](/Davinci_Portfolio/assets/IHMC/foot_off.jpg)

**Photo of the composite foot pad and mold**
![foot pad](/Davinci_Portfolio/assets/IHMC/20210630_Nadia_Parts_LowRes_17.jpg)

**Implementation**
## NADIA Movement Test
<iframe width="720" height="480" src="/Davinci_Portfolio/assets/IHMC/media11.mp4" frameborder="0" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<!-- ![Jump Collage](/Davinci_Portfolio/assets/IHMC/2021_Nadia_JumpCollage.jpg) -->
**Display of large range of motion of the Nadia legs**
![BendKick](/Davinci_Portfolio/assets/IHMC/20210630_Nadia_01_BendKick_Small.png)


# Other NADIA Projects

**Carbon Fiber process**
I helped develop a carbon fiber laying process that solved issues presented from previous carbon fiber laying processes. The previous process of creating the shell laid the carbon fiber inside of an outer mold with an inflation system that compressed the layers from the inside. That process would create imperfections on the inside surface that needed constant sanding and grinding in order to not conflict with the components housed inside. 

**Photo of the carbon fiber thigh with components inside**
![carbon thigh](/Davinci_Portfolio/assets/IHMC/20210630_Nadia_Parts_LowRes_06.jpg)

The new process involved creating a printable inner mold that would collapse inward for easy release and removal. The carbon fiber would be layered over the mold and vacuum sealed for curing. After the part is cured, the core mold would be collapsed and removed in pieces. This allowed us to easily fine tune the topology of the inner surface of the shell, reducing the amount of post processing needed. 

**Photo of the inner surface of the finished thigh shell**
![inner carbon thigh](/Davinci_Portfolio/assets/IHMC/20210630_Nadia_Parts_LowRes_11.jpg)

**Photo of me with leg assembly**
![part](/Davinci_Portfolio/assets/IHMC/me_with_leg.jpg)


**Group photo of the IHMC lab**
![lab_photo](/Davinci_Portfolio/assets/IHMC/ihmc_lab.png)
<!-- 
<!-- * [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
* [Markdown Guide](https://www.markdownguide.org/cheat-sheet/)
* [GitHub Flavored Markdown Spec](https://github.github.com/gfm/) --> 

---
<!-- 
# This is the h1 text
## This is the h2 text
### This is the h3 text
#### This is the h4 text
##### This is the h5 text
###### This is the h6 text

**Bold Text in the post will look like:**<br>
**This text is Bold**

**Italic Text in the post will look like:**<br>
*This text is Italic*

> Quotes on your post will look like this

`Codes on your post will look like this`

**Link in the post will look like:**<br>
[This is a link](#) -->

<!-- **Team Members**
* Haozhi Zhang, Devesh Bhura, Davin Landry, Kevin Nella, Daelan Roosa -->

<!-- ![Team image](/Davinci_Portfolio/assets/images/Vestibular_team.jpg) -->
<!-- 
**Generally, there are two types of tasks that our controlling of ping-pong ball can be achieved:**

1. Follow a line trajectory drawn on a white board.
2. Follow the path solved by our maze solver algorithm, with a maze drawn on a white board. -->

<!-- ### ROS Architecture
![arch image](/Davinci_Portfolio/assets/images/bal_arch.png)

### Controls diagram
![control image](/Davinci_Portfolio/assets/images/control_diagram.png) -->


<!-- ### Position Control
<iframe src="/Davinci_Portfolio/assets/videos/pushball.gif" width="600" height="360" frameBorder="0" class="giphy-embed" allowFullScreen></iframe> -->


<!-- **Computer Vision:**<br>
An intel Realsense D435i camera is used detect the realtime location of the ball and the marks on the board. It does this by color thresholding the colors orange, blue, pink, and purple for the ball, waypoint 1, waypoint 2, and the maze respectivly. The vision pipeline processes and extracts the data by creating a pixel mask, calculating the contrours, and extracting the centroids of those contours. The ball coordinates are published as a Ball_Pose() msg to the ball_pose topic. The maze mask data is passed to the service callbacks relating to the maze_follow and line_follow services. It then draws all contours over image feed and displays the resulting images in realtime.

**Maze Solver Algorithm:**<br>
The Breadth First search method is used to solve the maze and generate a trajectory for the ball to follow. To do so, the algorithm computes two cost maps, one where the points farthest away from the walls of the maze are assigned the lowest value, and another cost map that assigns higher value to the points furthest away from the starting point. The algorithm adds these two maps and does gradient descent from the start point to the goal, interating through the neighboring cells and finding a path.

**Future Improvements:**<br>
When we set our start position on the corners of board, sometimes the ball is hard to be balanced initially and could cause drastic motion of robot arm. One way to solve this issue might be adding more dimensions in our control by using more joints to achieve more dynamical balance when putting the ball in any position. -->

<!-- ![arch image](/Davinci_portfolio/assets/images/bal_arch.jpg)

![control image](/Davinci_portfolio/assets/images/control_diagram.jpg) -->
<!-- 
<!-- ## Line Following
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/videos/line_follow.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->
<!-- 
## NU Path Follow
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/videos/NU_Follow.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->

<!-- **YouTUbe Videos will look like:**<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/jTPXwbDtIpA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->