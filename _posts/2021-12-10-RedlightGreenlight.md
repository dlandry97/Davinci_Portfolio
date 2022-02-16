---
title: Redlight Greenlight Game
layout: post
post-image: "/Davinci_Portfolio/assets/RLGL/RLGLEric.gif"
description: I made an interactive Redlight Greenlight game from the hit Netflix series Squid Game. 
tags:
- Computer Vision
- Tracking
- Game
---
## Redlight Greenlight
For this project I created the computer vision system and the interactive game mechanics for redlight greenlight. Redlight Greenlight is the kids game where a seeker player tries to catch the other players moving while they try to cross a field. When the seeker calls "greenlight", the seeker covers their eyes while the other players are able to move across the field to reach the other side. Once the seeker calls "redlight", they uncover their eyes and the other players must freeze in place to not get caught moving by the seeker. If a player is caught moving during the redlight phase, they are eliminated from the game by the seeker.

**Game mechanics**<br>
To develop this game into a project, I chose to replace the role of the seeker with a robot. This robot would watch the players, call out the redlight/greenlight phases, eliminate players, and keep score with no assistance from humans. The players would start at a distance from the robot and try to get close to the robot without being eliminated. If they are caught moving during the wrong phase, they would lose one of three lives. The game would end when the players lose all lives or they reach the robot. 

**Computer vision**<br>
 I used the python libraries OpenCV, ROS, and pyrealsense2 to create the image processing pipeline for tracking the players. I used color recognition to identify the contours of the players and track their movements. Movement detection was determined by a change in position of the centroid of the contoured area beyond a certain threshold. The player's distance from the goal was detected by utilizing the Intel Realsense D435i's depth perception camera. 

![tracking](/Davinci_portfolio/assets/RLGL/playertracking.jpg)

**Integration**<br>
To combine the computer vision and game algorithm together, I used the ROS python package. I made a node to manage the image pipeline and send the data to another node that manages the game mechanics and score. The game node would use state machines and timers to manage the game phases and data triggers to keep track of the score. There is an additional node to manage the sound ques to prevent process halting issues.



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

<!-- ### ROS Architecture
![arch image](/Davinci_Portfolio/assets/images/bal_arch.png)

### Controls diagram
![control image](/Davinci_Portfolio/assets/images/control_diagram.png) -->


<!-- ### Position Control
<iframe src="/Davinci_Portfolio/assets/videos/pushball.gif" width="600" height="360" frameBorder="0" class="giphy-embed" allowFullScreen></iframe> -->





<!-- ![control image](/Davinci_portfolio/assets/images/control_diagram.jpg) -->

## Video Presentation
<iframe width="560" height="315" src="https://youtu.be/3N2Qco0lPuc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Player Elimination
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/RLGL/elimination.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Full game
<iframe width="560" height="315" src="/Davinci_Portfolio/assets/RLGL/Rolling.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<!-- **YouTUbe Videos will look like:**<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/jTPXwbDtIpA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->