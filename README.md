# Projects #
Headings link to GitHub projects.
## Robotics Projects ##

###[roshask](https://github.com/acowley/roshask)###
roshask is the [ROS](http://www.ros.org) Haskell library written by Anthony Cowley. I added support for [ROS service](http://wiki.ros.org/Services) clients. This [pull request](https://github.com/acowley/roshask/pull/24) has the commits that were merged. If you are curious about the development process, here is a [code review](https://github.com/acowley/roshask/pull/22) with feedback from Anthony.
###Nerfinator###
Nerfinator is a robotic Nerf sentry built with Sadegh Asefi as our EE 125 final project. It uses the Kinect RGBD camera to aim at faces at varying distances. It also can use a laser pointer to correct its aim. Two minute [video overview](https://www.youtube.com/watch?v=oau05MdCPMc). [Playlist](https://www.youtube.com/watch?v=3zx1phhTI8c&list=PLj1b-zmkThBO8FdYdLjTq-sJV3GInXYMh) of all videos.
###[Learning from Demonstration](https://github.com/rgleichman/rapprentice)###
One approach to teaching a robot how to perform a task is to directly demonstrate the task to the robot by manually moving it's arms and commanding its gripper like a puppet. The robot records the actions the human has demonstrated, along with information about the state of the object being manipulated. The robot can then use the recorded demonstration to manipulate objects in novel environments.

A variation of this approach is to record multiple demonstrations with the object to be manipulated placed in varying initial states. When asked to preform a task, the robot picks one of the many recorded demonstrations. I helped develop a bootstrapping algorithm that enables the robot to learn from its past successes and failures by improving its choice of demonstration.

For a very specific simulated knot tying task, bootstrapping improved the success rate from 60% to 98%. I worked directly with Or Weizman, Ankush Gupta, and Dylan Hadfield-Menell on developing bootstrapping. This work built upon work done by John Schulman, Jonathan Ho, and Cameron Lee ([videos and pdf of their paper](http://rll.berkeley.edu/isrr2013lfd/)). This work was done in Pieter Abbeel's lab at UC Berkeley. The lab's current learning from demonstration work can be found [here](http://lfd.readthedocs.org/en/latest/).
###Robot Gripper Optical Sensors###
Pieter Abbeel's lab received from an external lab a few optical sensors for the PR2's grippers. On one gripper pad is an array of four IR light sensors. On the the other are four matching IR LED's. If the amount of light received by one of the sensors decreases, then it indicates there is something inside the gripper. These could possibly be used to improve grasping or sense the shape of objects.

For this project I wrote a simple 2D gripper simulator in Haskell using Helm ([GitHub](https://github.com/rgleichman/sense)).
I also started working on using these sensors with the PR2 using ROS and roshask ([GitHub](https://github.com/rgleichman/uwsensor_demos)). Unfortunately, these experimental sensors broke often and had to be sent back before I could make much progress.
