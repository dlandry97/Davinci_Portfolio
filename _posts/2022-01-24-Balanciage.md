---
title: Balanciaga
layout: post
post-image: "/Davinci_portfolio/assets/images/balanciaga.jpg"
description: The goal of this project is to control a ping-pong ball by using Franka Panda robot to manipulate a white board. This is a ROS project developed as part of ME495 - Embedded Systems in Robotics course at Northwestern University.
tags:
- Robotics
- Post
- Engineering
- Balance
---

The project integrates two main portions. First part is the perception: we use real sense camera as our sensor to capture the transient positions of ball and board, and using OpenCV library processes the sensing images. Second part is the control: there are two PD controllers we are implementing to control the ping-pong ball following the target trajectory on the white board. The higher level control loop takes ball positions as input and outputs desired angles of corresponding two arm joints. Then the updated joint angles received by the low level control loop. By tuning PD gains, this loop is able to send desired efforts to robot arm through ros_control topic.

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

**Team Members**
* Haozhi Zhang, Devesh Bhura, Davin Landry, Kevin Nella, Daelan Roosa

![Team image]("/Davinci_portfolio/assets/images/Vestibular_team.jpg")

**Generally, there are two types of tasks that our controlling of ping-pong ball can be achieved:**

1. Follow a line trajectory drawn on a white board.
2. Follow the path solved by our maze solver algorithm, with a maze drawn on a white board.

### ROS Architecture
![arch image]("/Davinci_portfolio/assets/images/bal_arch.jpg")

### Controls diagram
![control image]("/Davinci_portfolio/assets/images/control_diagram.jpg")


### Position Control
<iframe src=/Davinci_portfolio/assets/videos/pushball.gif width="480" height="259" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>


**Computer Vision:**<br>
An intel Realsense D435i camera is used detect the realtime location of the ball and the marks on the board. It does this by color thresholding the colors orange, blue, pink, and purple for the ball, waypoint 1, waypoint 2, and the maze respectivly. The vision pipeline processes and extracts the data by creating a pixel mask, calculating the contrours, and extracting the centroids of those contours. The ball coordinates are published as a Ball_Pose() msg to the ball_pose topic. The maze mask data is passed to the service callbacks relating to the maze_follow and line_follow services. It then draws all contours over image feed and displays the resulting images in realtime.

**Maze Solver Algorithm:**<br>
The Breadth First search method is used to solve the maze and generate a trajectory for the ball to follow. To do so, the algorithm computes two cost maps, one where the points farthest away from the walls of the maze are assigned the lowest value, and another cost map that assigns higher value to the points furthest away from the starting point. The algorithm adds these two maps and does gradient descent from the start point to the goal, interating through the neighboring cells and finding a path.

**Future Improvements:**<br>
When we set our start position on the corners of board, sometimes the ball is hard to be balanced initially and could cause drastic motion of robot arm. One way to solve this issue might be adding more dimensions in our control by using more joints to achieve more dynamical balance when putting the ball in any position.

<!-- ![arch image](/Davinci_portfolio/assets/images/bal_arch.jpg)

![control image](/Davinci_portfolio/assets/images/control_diagram.jpg) -->

## Line Following
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/videos/line_follow.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## NU Path Follow
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/videos/NU_Follow.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Maze Solving
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/videos/Maze_follow.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<!-- **YouTUbe Videos will look like:**<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/jTPXwbDtIpA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->