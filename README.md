<h1>Laboratory 3: Navvis Sensor and Bag</h1>
<h2>Overview</h2>
<p>This package builds the robot with its sensors and views the sensor data from the ROS bag file of Glennan 5th Floor in RVIZ.</p>

<h2>Instructions for Launch</h2>
<p>Open a new terminal and configure ROS.</p>
<p>Pull this package and the navvis_description package into your workspace.</p>
    <ul>
        <li>This package depends on the navvis_description package.</li>
    </ul>
<p>Make sure to have the basic short version of the Glennan 5th Floor bag file downloaded to Downloads.</p>
<p>There are three different launch files to start RVIZ.</p>
    <ol>
        <li>To view the sensor data with robot</li> 
            <ul>
                <li>Edit the lab3.launch file and ensure the path to the bag file has /home/< your-username >.</li>
                <li>Run the command: roslaunch navvis_sensor lab3.launch</li>
                <li>This roslaunch command takes the arguments:</li>
                    <ul>
                        <li>use_xacro:=true|false which specifies if the xacro file or urdf file is used.</li>
                        <li>use_joint_state_publisher_gui:=true|false which specifies if the joint_state_publisher GUI is opened.</li>
                        <li>use_robot_state_publisher:=true|false which specifies if the robot_state_publisher node or the static transformation is used.</li>
                    </ul>
            </ul>
        <li>To only view the robot description, use the following command:</li>
            <ul>
                <li>roslaunch navvis_sensor lab2_original.launch</li>
                <li>This roslaunch command takes the arguments:</li>
                    <ul>
                        <li>use_xacro:=true|false which specifies if the xacro file or urdf file is used.</li>
                        <li>use_joint_state_publisher_gui:=true|false which specifies if the joint_state_publisher GUI is opened.</li>
                    </ul>
            </ul>
        <li>To view the robot description which excludes the base_link and imu elements but can read ROS bags, use the following command:</li>
            <ul>
                <li>roslaunch navvis_description display.launch</li>
                <li>This roslaunch command takes the arguments:</li>
                    <ul>
                        <li>use_xacro:=true|false which specifies if the xacro file or urdf file is used.</li>
                        <li>use_joint_state_publisher_gui:=true|false which specifies if the joint_state_publisher GUI is opened.</li>
                        <li>use_robot_state_publisher:=true|false which specifies if the robot_state_publisher node or the static transformation is used.</li>
                    </ul>
            </ul>
    </ol>

        
            
            