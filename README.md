# TASK-2
Install the arm package
# 1- Preparing ROS
* Create a workspace by using catkin_make

`mkdir -p ~/catkin_ws/src`

`cd ~/catkin_ws/`

`catkin_make`

` cd ~/catkin_ws/src`

![‏‏لقطة الشاشة (262)](https://user-images.githubusercontent.com/110434554/182949313-84f79359-9422-4e8e-8dc2-a32765b55afd.png)

# 2- Installing the package arduino_robot_arm

Add the “arduino_robot_arm” package to “src” folder

`git clone https://github.com/smart-methods/arduino_robot_arm `

* install all the dependencies

`cd ~/catkin_ws`

`rosdep install --from-paths src --ignore-src -r -y`

![‏‏لقطة الشاشة (256)](https://user-images.githubusercontent.com/110434554/182949486-152443b6-371f-4c50-8384-436fc6dd4ddb.png)

`sudo apt-get install ros-noetic-moveit`

![‏‏لقطة الشاشة (259)](https://user-images.githubusercontent.com/110434554/182949566-febe96a5-e128-45bc-923c-1fcfb36926e5.png)

`sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui`

`sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher`

![‏‏لقطة الشاشة (258)](https://user-images.githubusercontent.com/110434554/182949909-b8ce456e-35de-4b90-baed-5df5570f0ab2.png)

`sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control`

![‏‏لقطة الشاشة (257)](https://user-images.githubusercontent.com/110434554/182949980-48755de3-0132-4960-8013-d769453c7067.png)

`sudo nano ~/.bashrc`

* at the end of the (bashrc) file add the follwing line

(source /home/esraa/catkin_ws/devel/setup.bash)
then 
ctrl + o

`source ~/.bashrc`

![‏‏لقطة الشاشة (260)](https://user-images.githubusercontent.com/110434554/182950419-d8019901-fa4b-42a5-a29f-00de0bae99ff.png)

# 3-Controlling the motors

`roslaunch robot_arm_pkg check_motors.launch`

![‏‏لقطة الشاشة (261)](https://user-images.githubusercontent.com/110434554/182950448-6c547771-b132-4e6a-9117-6a8a547d1f80.png)
