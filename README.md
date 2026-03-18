# Unitree Go2 ROS 2 Workspace

## Introduction
This repository hosts the code and resources for integrating the Unitree Go2 robot with ROS 2. The Unitree Go2 brings advanced robotics technology to your fingertips, and with this workspace, you can leverage its full potential within the ROS 2 ecosystem.

## Requirements
- **ROS 2 Foxy Fitzroy** or higher
- **Ubuntu 20.04** (recommended)
- Unitree Go2 robot

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/2747179309/go2_ros2_ws.git
   cd go2_ros2_ws
   ```
2. Install dependencies:
   ```bash
   sudo apt update
   sudo apt install -y ros-foxy-<package_name>
   ```
3. Build the workspace:
   ```bash
   colcon build
   source install/setup.bash
   ```

## Usage
- Launch the robot:
   ```bash
   ros2 launch unitree_go2_bringup bringup.launch.py
   ```
- Control the robot using:
   ```bash
   ros2 topic pub /cmd_vel geometry_msgs/msg/Twist "{ linear: { x: 0.1, y: 0.0, z: 0.0 }, angular: { x: 0.0, y: 0.0, z: 0.1 } }"
   ```

## Features
- Real-time control of the Unitree Go2
- Sensor data streaming and processing
- Easy navigation and mapping integration

## Contributing
We welcome contributions! Please fork the repository, make your changes, and submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- Special thanks to Unitree for providing the Go2 robot.
- Thanks to the ROS community for their ongoing support.

## Contact
For inquiries, contact [Your Name](mailto:your_email@example.com).