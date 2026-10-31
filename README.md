Environment: Ubuntu 26.4 WSL for learning and ROS2 ROS 2 Lyrical Luth (LTS).
Install ROS2 and add "source /opt/ros/lyrical/setup.bash" in .bashrc so that it takes source every time linux starts.
---------------------------------------------------------------------------------------------------------
To create python package use
ros2 pkg create <pkg_name> --build_type ament_python --dependencies rclpy
---------------------------------------------------------------------------------------------------------------
ament is a build system that can help in building python and c++
rclpy is python libs to write python code in ROS2

----------------------------------------------------------------------------------------------------------------------------
To create cpp packages use 
ros2 pkg create <pkg_name> --build-type ament_cmake --dependencies rclcpp

To build use
colcon build --packages-select <pkg_name>

What is a Package ?
A package is an independent unit inside your application. for example Hardware control pkg, motion pkg, camera pkg.

What is a Node?
Nodes are programs inside a package, A code can launch independently. It is just like class in (OOP). Two nodes can not have same name.
