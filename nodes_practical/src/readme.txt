- Pilotin Thedy, Dzodjou Chendjou (512224)
- Daniel Randy, Azmhau (511962)
- Eric Junior, Tchassem Ngounou (509561)


1-
student@ubuntu:~/catkin_ws/src/nodes_practical/src$ rostopic show geometry_msgs/twist
rostopic is a command-line tool for printing information about ROS Topics.

Commands:
	rostopic bw	display bandwidth used by topic
	rostopic delay	display delay of topic from timestamp in header
	rostopic echo	print messages to screen
	rostopic find	find topics by type
	rostopic hz	display publishing rate of topic    
	rostopic info	print information about active topic
	rostopic list	list active topics
	rostopic pub	publish data to topic
	rostopic type	print topic or field type

Type rostopic <command> -h for more detailed usage, e.g. 'rostopic echo -h'


2- 
student@ubuntu:~/catkin_ws/src/nodes_practical/src$ roslaunch sjtu_drone simple.launch
... logging to /home/student/.ros/log/63b07f08-bfbd-11ea-b1b2-000c29bbbcc5/roslaunch-ubuntu-5930.log
Checking log directory for disk usage. This may take awhile.
Press Ctrl-C to interrupt
Done checking log file disk usage. Usage is <1GB.

started roslaunch server http://ubuntu:36325/

SUMMARY
========

PARAMETERS
 * /gazebo/enable_ros_network: True
 * /rosdistro: melodic
 * /rosversion: 1.14.3
 * /use_sim_time: True

NODES
  /
    gazebo (gazebo_ros/gzserver)
    gazebo_gui (gazebo_ros/gzclient)

ROS_MASTER_URI=http://localhost:11311

process[gazebo-1]: started with pid [5945]
process[gazebo_gui-2]: started with pid [5947]
Gazebo multi-robot simulator, version 9.0.0
Copyright (C) 2012 Open Source Robotics Foundation.
Released under the Apache 2 License.
http://gazebosim.org

[Wrn] [GuiIface.cc:199] g/gui-plugin is really loading a SystemPlugin. To load a GUI plugin please use --gui-client-plugin 
Gazebo multi-robot simulator, version 9.0.0
Copyright (C) 2012 Open Source Robotics Foundation.
Released under the Apache 2 License.
http://gazebosim.org

[ INFO] [1594068540.154069809]: Finished loading Gazebo ROS API Plugin.
[ INFO] [1594068540.165248948]: Finished loading Gazebo ROS API Plugin.
[Msg] Waiting for master.
[ INFO] [1594068540.170722654]: waitForService: Service [/gazebo/set_physics_properties] has not been advertised, waiting...
[Msg] Waiting for master.
[ INFO] [1594068540.180212439]: waitForService: Service [/gazebo_gui/set_physics_properties] has not been advertised, waiting...
[Msg] Connected to gazebo master @ http://127.0.0.1:11345
[Msg] Connected to gazebo master @ http://127.0.0.1:11345
[Msg] Publicized address: 192.168.255.134
[Msg] Publicized address: 192.168.255.134
[Wrn] [msgs.cc:1852] Conversion of sensor type[sonar] not supported.
[Err] [InsertModelWidget.cc:405] Missing model.config for model "/home/student/gazebo_ws/gazebo_models/.hg"
[ INFO] [1594068550.376657546]: The IMU plugin has been loaded!
[ INFO] [1594068550.421123513]: The Sonar plugin has been loaded!
[Wrn] [Event.cc:61] Warning: Deleting a connection right after creation. Make sure to save the ConnectionPtr from a Connect call
[ INFO] [1594068554.430423240]: The camera plugin has been loaded!
[ INFO] [1594068554.433826021]: The camera plugin has been loaded!
[ INFO] [1594068554.462031850]: The drone plugin is loading!
[ INFO] [1594068554.466556622]: Using cmd_topic /cmd_vel.
[ INFO] [1594068554.468960419]: find the position control topic!
[ INFO] [1594068554.471130937]: Using imu information on topic /drone/imu as source of orientation and angular velocity.
[ INFO] [1594068554.474794829]: find the takeoff topic
[Wrn] [msgs.cc:1852] Conversion of sensor type[sonar] not supported.
[Wrn] [msgs.cc:1852] Conversion of sensor type[sonar] not supported.
[Wrn] [Publisher.cc:141] Queue limit reached for topic /gazebo/default/pose/local/info, deleting message. This warning is printed only once.
[Wrn] [msgs.cc:1852] Conversion of sensor type[sonar] not supported.
[Wrn] [Publisher.cc:141] Queue limit reached for topic /gazebo/default/user_camera/pose, deleting message. This warning is printed only once.
[ INFO] [1594068656.342823012]: 
Quadrotor takes off!!
[ INFO] [1594068656.460387946, 0.030000000]: waitForService: Service [/gazebo/set_physics_properties] is now available.
[Wrn] [Publisher.cc:141] Queue limit reached for topic /gazebo/default/physics/contacts, deleting message. This warning is printed only once.
[ INFO] [1594068656.826222942, 0.362000000]: Physics dynamic reconfigure ready.
Entering flying model!
[ INFO] [1594068657.845429886, 1.004000000]: 
Quadrotor lands!!
Landed!
[Wrn] [Publisher.cc:141] Queue limit reached for topic /gazebo/default/pose/info, deleting message. This warning is printed only once.

3-
student@ubuntu:~/catkin_ws/src/nodes_practical/src$ rosrun  nodes_practical move.py
Input your speed:5
Type your distance:4
Foward?: 1


