# Robo_Chase_the_Ball

This project launches a robot in a designed gazebo world environment. The robot motion is controlled by a node called 
"ball_chaser". This node drives the robot towards the white ball captured by the camera mounted on the robot. 

## Execution
Create the required directories for the workspace:
```
mkdir -p catkin_ws/src
```
Initialize the workspace and build the project:
```
cd src
catkin_init_worksapce
cd ..
catkin_make
```
Source the setup file:
```
source devel/setup.bash
```
Run the gazebo_world related nodes:
```
roslaunch my_robot world.launch
```
Run the ball_chaser node:
```
roslaunch my_robot world.launch 
```
In order to run the view in rviz from the camera point of view run the following command:
```
rosrun rqt_image_view rqt_image_view
```

If the white ball in the in the field of view of the camera, the robot does not move or stops moving:

![](https://github.com/shmousavi65/Robo_Chase_the_Ball/blob/master/Capture1.PNG)

If the white ball in the in the field of view of the camera, the robot moves toward it:

![](https://github.com/shmousavi65/Robo_Chase_the_Ball/blob/master/Capture2.PNG)

![](https://github.com/shmousavi65/Robo_Chase_the_Ball/blob/master/Capture3.PNG)
