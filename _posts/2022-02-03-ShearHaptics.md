---
title: Shear Haptics VR Controller
layout: post
post-image: "/Davinci_Portfolio/assets/ShearHaptics/prototype2.gif"
description: A virtual reality haptic controller that uses shear grip movement to simulate torque and moments when interacting with large objects in VR.
tags:
- Robotics
- Engineering
- VR
- Design
- In_Progress
- Northwestern
---

This project is still in progress.
The two main portions of this project include the design the mechanical structure of the device, and the integration of the haptic feedback with a virtual environment. 

**Prototyping**

The general goal for the design was to create a shear movment about the controller grip with minimal actuators and a comfortable form as a handheld device. To achieve the linear motion of the grips, many actuation schemes were considered such as; linear actuators, worm gears, gears, belt drives. The decided mechanism was a timing belt system actuated by a single high torque servo motor. The belt driven system gives the advantage of displacing the motor location away from the handle while still achieving strong linear force through the grips. The timing belt attaches to a set of carts guided by steel shaft rails. These shafts would function as a skeletal structure of the device as well as guide the grips in a linear path up and down the device. The second prototype increases efficiency and confort by slimming down the size of the mechanism while increasing the size of the grips.

##### Prototype 1 test
![Prototype 1](/Davinci_Portfolio/assets/ShearHaptics/prototype1.gif)


**Actuation**

The actuation of the device is provided by a single 35kg/cm servo motor controlled by an arduino uno microcontroller. The servo drives a timing belt that attaches to and drives the grips. 
Each grip is designed to have a -10mm to 10mm travel range.

**Tracking**
I plan to use a HTC vive tracker attached to the top of the device to obtain tracking data for VR application.

**Interfacing**
I am using Unity game enigne to create a VR demo environemnt to integrate with the device. I'm using serial communication to read and write signals from Unity to the arduino to sync up to impacts in VR to the haptic feedback of the controller.



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



<!-- ![Team image](/Davinci_Portfolio/assets/images/Vestibular_team.jpg) -->

<!-- **Generally, there are two types of tasks that our controlling of ping-pong ball can be achieved:**

1. Follow a line trajectory drawn on a white board.
2. Follow the path solved by our maze solver algorithm, with a maze drawn on a white board. -->

<!-- ### ROS Architecture
![arch image](/Davinci_Portfolio/assets/images/bal_arch.png)

### Controls diagram
![control image](/Davinci_Portfolio/assets/images/control_diagram.png) -->


<!-- ### Position Control
<iframe src="/Davinci_Portfolio/assets/videos/pushball.gif" width="600" height="360" frameBorder="0" class="giphy-embed" allowFullScreen></iframe> -->

<!-- 
**Computer Vision:**<br>
An intel Realsense D435i camera is used detect the realtime location of the ball and the marks on the board. It does this by color thresholding the colors orange, blue, pink, and purple for the ball, waypoint 1, waypoint 2, and the maze respectivly. The vision pipeline processes and extracts the data by creating a pixel mask, calculating the contrours, and extracting the centroids of those contours. The ball coordinates are published as a Ball_Pose() msg to the ball_pose topic. The maze mask data is passed to the service callbacks relating to the maze_follow and line_follow services. It then draws all contours over image feed and displays the resulting images in realtime.

**Maze Solver Algorithm:**<br>
The Breadth First search method is used to solve the maze and generate a trajectory for the ball to follow. To do so, the algorithm computes two cost maps, one where the points farthest away from the walls of the maze are assigned the lowest value, and another cost map that assigns higher value to the points furthest away from the starting point. The algorithm adds these two maps and does gradient descent from the start point to the goal, interating through the neighboring cells and finding a path.

**Future Improvements:**<br>
When we set our start position on the corners of board, sometimes the ball is hard to be balanced initially and could cause drastic motion of robot arm. One way to solve this issue might be adding more dimensions in our control by using more joints to achieve more dynamical balance when putting the ball in any position. -->

<!-- ## Line Following
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/videos/line_follow.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## NU Path Follow
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/videos/NU_Follow.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Maze Solving
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/videos/Maze_follow.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->

<!-- **YouTUbe Videos will look like:**<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/jTPXwbDtIpA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->