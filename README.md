# homework3

PUNTO 1-c
Runnare gazebo: roslaunch iiwa_gazebo iiwa_gazebo_circular_object.launch
Runnare il nodo blobDetector: rosrun opencv_ros opencv_ros_node


PUNTO 2-a/2-b -------> ATTENZIONE CONTROLLARE CHE I CONTROLLORI CARICATI IN IIWA_GAZEBO_ARUCO.LAUNCH SIANO I VELOCITYINTERFACE 
Runnare gazebo: roslaunch iiwa_gazebo iiwa_gazebo_aruco.launch
Runnare l'aruco: roslaunch aruco_ros usb_cam_aruco.launch camera:=/iiwa/camera1
Runnare il controllore: rosrun kdl_ros_control kdl_robot_vision_control ./src/iiwa_stack/iiwa_description/urdf/iiwa14.urdf


PUNTO 2-c -------> ATTENZIONE CONTROLLARE CHE I CONTROLLORI CARICATI IN IIWA_GAZEBO_ARUCO.LAUNCH SIANO GLI EFFORT CONTROLLERS
Runnare gazebo: roslaunch iiwa_gazebo iiwa_gazebo_aruco.launch
Runnare l'aruco: roslaunch aruco_ros usb_cam_aruco.launch camera:=/iiwa/camera1
Runnare il controllore: rosrun kdl_ros_control kdl_robot_test ./src/iiwa_stack/iiwa_description/urdf/iiwa14.urdf
