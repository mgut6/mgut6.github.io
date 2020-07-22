---
title: "Quadcopter"
excerpt: "Remote controlled, self-leveling quadcopter<br/><img src='/images/500x300.png'>"
collection: portfolio
---
Video<br/><br/>
During the summer of 2020 I undertook a project to build my own remote controlled quadcopter. While researching the workings of quadcopters, I learned about IMUs and the process of how a quadcopter levels itself. Deciding upon an IMU consisting of a 3-axis gyroscope and 3-axis accelerometer, I purchased the necessary hardware to begin building. I chose an Arduino Uno to serve as the flight controller due to its ease of programming and its large current output compared to the Arduino mini.<br/>
<center><img src ='/images/500x300.png'><br/>
<em>Mounted Arduino UNO</em></center><br/>
I mounted the Arduino above the surface of the frame in order to place the IMU at the center of the quadcopter. That way the vibrations from the motors would have the smallest effect on the IMU. The mount for the Arduino and for the IMU were both designed in Solidworks and then 3D printed. A 3s lipo battery was used to power the quadcopter, directly powering the ESCs, motors, and the Arduino. The 5V pin on the Arduino was used to power both the IMU and the receiver, separating them from the ~12V circuit powering the motors. Additionally, an indicator LED was mounted on the front of the quadcopter to indicate status while calibrating the gyro and to indicate low battery during flight. <br/>
<center><img src ='/images/500x300.png'><br/>
<em>MPU-6050 Gyroscope/Accelerometer</em></center><br/>
I chose the MPU-6050 gyro/accelerometer because it contained everything I needed for the IMU on one board and was 5V compatible. The IMU mainly used the motion detected by the gyro to determine the quadcopter position. The accelerometer was used to determine the quadcopter's initial position upon powering on and to add a small correction for the drift of the gyro during flight.
