---
title: Humanoid Robot Feet
layout: post
post-image: "/Davinci_Portfolio/assets/videos/pushball.gif"
description: This project involves the research and design of feet for the NADIA robot, a hydraulic powered humanoid robot in development at The Institute for Human and Machine Cognition (IHMC).
tags:
- Robotics
- Engineering
- Design
- Research
- IHMC
---

This project started as a literature review of robotic feet for bipedal humanoid robots. There was also extensive reserach in what type of sensor would be ideal for robot feet considering COP and ground sensing. The findings of the literature review and sensor reserach were used to design many novel prototype feet that were considered for the NADIA robot. This led to the specification, commision, and testing of a 6-axis force/torque sensor. The testing and implimentation of the foot sensor continued throughout my time at the IHMC.



**Literature Review**
The literature review was focused on dynamic robot feet both actuated and passive with the goal to increase efficiency and ability for robotic bipedal locomotion. This review covered a humanoid robots from all over the world including Atlas, ASIMO, HRP, LOLA, Sarcos, TORO, Cassie, Digit, WABIAN, and many more.


**Sensor**
Robotic foot sensors need to be able to sense center of pressure. To do this, you need to be able to sense 3 axis of force; x-moment, y-moment, z-axial. 


**Design and Prototyping**
![cad foot](/Davinci_Portfolio/assets/IHMC/cad_foot.png)
![plastic foot](/Davinci_Portfolio/assets/IHMC/plastic_foot.jpg)
![foot](/Davinci_Portfolio/assets/IHMC/foot_off.jpg)

**Implimentation**
## NADIA Movement Test
<iframe width="720" height="480" src="/Davinci_Portfolio/assets/IHMC/media11.mp4" frameborder="0" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

![Jump Collage](/Davinci_Portfolio/assets/IHMC/2021_Nadia_JumpCollage.jpg)
![BendKick](/Davinci_Portfolio/assets/IHMC/20210630_Nadia_BendKick_Small.png)
![carbon thigh](/Davinci_Portfolio/assets/IHMC/20210630_Nadia_Parts_LowRes_06.jpg)
![inner carbon thigh](/Davinci_Portfolio/assets/IHMC/20210630_Nadia_Parts_LowRes_11.jpg)
![foot pad](/Davinci_Portfolio/assets/IHMC/20210630_Nadia_Parts_LowRes_17.jpg)

![part](/Davinci_Portfolio/assets/IHMC/me_with_leg.jpg)

![lab_photo](/Davinci_Portfolio/assets/IHMC/ihmc_lab.png)
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