# Robbie Gleichman #
###[My GitHub](https://github.com/rgleichman)###

# Projects #
Headers link to GitHub projects. This list is not exhaustive, but it does include most of my public GitHub projects.


## Recent Projects ##

### [Glance](https://github.com/rgleichman/glance) (a visual representation of Haskell) ##
Glance is my attempt at representing Haskell visually. It is designed (at least initially) to be automatically generated from textual Haskell code. [Here](https://docs.google.com/document/d/1iLP4izhdJU2qlU2nasb7dfQAm7hytcl5IYcgi7dXHSk/edit?usp=sharing) is a first draft of a Google Doc introducing the language; please comment. Glance is currently in the design stage.


### [smock](https://github.com/rgleichman/smock) ###
smock is a function mocking framework I wrote for Haskell. It is experimental and not very practical; however, I did learn about overlapping instances and data families in Haskell.

### [Haskell immutable skip list](https://github.com/rgleichman/skip) ###
This is an experimental module I wrote that can be used for quickly searching through a, possibly infinite, ascending list. When I tested it, the skip list was faster at creating its searchable data structure than [Data.Set in containers](http://hackage.haskell.org/package/containers-0.5.6.3/docs/Data-Set.html). The skip list's data structure also used less memory. However, the skip list was slower at finding elements, so it would only be faster overall if your code does few searches relative to list size.

## Robotics Projects ##

###[roshask](https://github.com/acowley/roshask)###
roshask is the [ROS](http://www.ros.org) Haskell library written by Anthony Cowley. I added support for [ROS service](http://wiki.ros.org/Services) clients. This [pull request](https://github.com/acowley/roshask/pull/24) has the commits that were merged. If you are curious about the development process, here is a [code review](https://github.com/acowley/roshask/pull/22) with feedback from Anthony.
###Nerfinator###
Nerfinator is a robotic Nerf sentry built by Sadegh Asefi and myself as our EE 125 (Introduction to Robotics) final project. It uses the Kinect RGBD camera to aim at faces at varying distances. It also can use a laser pointer to correct its aim. Here is a two minute [video overview](https://www.youtube.com/watch?v=oau05MdCPMc), and a YouTube [playlist](https://www.youtube.com/watch?v=3zx1phhTI8c&list=PLj1b-zmkThBO8FdYdLjTq-sJV3GInXYMh) with all of the videos.
###[Learning from Demonstration](https://github.com/rgleichman/rapprentice)###
One approach to teaching a robot how to perform a task is to directly demonstrate the task to the robot by manually moving it's arms and controlling its gripper. The robot records the actions the human has demonstrated, along with information about the state of the object being manipulated. The robot then uses the recorded demonstration to manipulate objects in novel environments.

A variation of this approach is to record multiple demonstrations, with the object to be manipulated placed in varying initial states. When asked to preform a task, the robot picks one of its many recorded demonstrations. I helped develop a bootstrapping algorithm that enables the robot to learn from its past successes and failures by improving its choice of demonstration.

For a very specific simulated knot tying task, the bootstrapping algorithm improved the robot's success rate from 60% to 98%. I worked directly with Or Weizman, Ankush Gupta, and Dylan Hadfield-Menell on developing bootstrapping. This work built upon work done by John Schulman, Jonathan Ho, and Cameron Lee ([videos and pdf of their paper](http://rll.berkeley.edu/isrr2013lfd/)). This work was done in Pieter Abbeel's lab at UC Berkeley, and the lab's current learning from demonstration work can be found [here](http://lfd.readthedocs.org/en/latest/).
###Robot Gripper Optical Sensors###
Pieter Abbeel's lab received from an external lab a few optical sensors for the PR2 robot grippers. On one gripper pad is an array of four IR light sensors. On the the other are four matching IR LED's. If the amount of light received by one of the sensors decreases, then it indicates there is something inside the gripper. These could be used to improve grasping or to sense the shape of objects.

For this project I wrote a simple 2D gripper simulator in Haskell using [Helm](http://helm-engine.org/) ([GitHub](https://github.com/rgleichman/sense)).
I also started working on using these sensors with the PR2 using ROS and roshask ([GitHub](https://github.com/rgleichman/uwsensor_demos)). Unfortunately, these experimental sensors broke often and had to be sent back before I could make much progress.
## Other Projects ##
###[ShopType](https://github.com/rgleichman/shoptype)###
[Link to play](http://rgleichman.github.io/shoptype)

ShopType is a typing game that was created in 2011 for Art 23 AC, a class that involved teaching Chinese speakers in Oakland CA how to use computers. Jeremy Blalock and I were the programmers for this game. I put this on GitHub in 2015; all commits are bug fixes.
###[Fixit](https://github.com/phoebesimon/fixit)###
Fixit was our group's project for CS 169 (Software Engineering). We (Phoebe Simon, Chris Turney, Frank Yü,  and I) collaborated with a UC Berkeley housing employee to make a new maintenance request website using Ruby on Rails. This project is notable for having very high test coverage.
###[Heartbeat](https://github.com/rgleichman/heartBeat)###
Heartbeat is an Android app I created that measures your heart rate. To use it, you place your phone's microphone directly on your chest, and the app listens for volume peaks. I wrote this while learning Android development.
###[Trontium Reactor](https://github.com/rgleichman/reactor)###
This code animates a color LED ring with an Arduino. A touch sensor switches animations. This project was for a friend's product video. Here is the [video](https://vimeo.com/88085657), including the animations I created.

Note: This site is created with GitHub pages ([GitHub source](https://github.com/rgleichman/rgleichman.github.io)).
