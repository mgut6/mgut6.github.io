---
title: "Cable Robot Simulation"
excerpt: "MATLAB simulation of a cable robot<br/><img src='/images/cable_robot_sim.PNG' width='500' height='300'>"
collection: portfolio
---
In the fall semester of 2020, I took a class in robotics that included a small group project as part of the course. My group decided to simulate a cable robot using MATLAB. The position of a cable robot is controlled by shortening and lengthening a series of cables attached to the robot on one end and a fixed base point on the other. We chose to control our simulated robot using inverse kinematics. Given a desired location, our MATLAB code calculated the required cable lengths to achieve this position.<br/>
<center><img src ='/images/cable_robot_diag.JPG' width="400" height="240"><br/>
<em>Diagram of cable robot kinematics (Bruckmann, Mikelsons, etc. 2008)</em></center><br/>
Unlike a robotic arm where the length of its joints limits its range of motion, a cable robot is limited by the tensions in its cables. For a cable robot to remain at a desired position, all forces and torques must balance. This becomes complicated because the cables must remain under a minimum level of tension to prevent sagging. Therefore, the major challenge in designing a cable robot is designing it to cover a large enough workspace i.e. large range of locations where a valid set of cable tensions exist.<br/>
<center><img src ='/images/cable_robot_wrkspc.png' width = "400" height="240"><br/>
<em>Workspace of an 8 cable robot</em></center><br/>
The project also incorporated computer vision as a means of guiding the position of the simulated cable robot. A checkered pattern was printed and attached to a clipboard which was tracked by a laptop webcam. Both the location and the orientation of the checker board were turned into translation and rotation in the simulation.<br/>
<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/acuXtbej174" frameborder="0" allowfullscreen="true" width="500" height="300"> </iframe>
</figure>
