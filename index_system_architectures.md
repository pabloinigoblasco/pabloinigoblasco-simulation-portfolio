# Pablo Iñigo Blasco - System Architecture & Integration Portfolio

Technical portfolio showcasing a selection of system architecture and integration projects in this area that I have been able to work on and that are publicly available or I have permission to show. This portfolio demonstrates expertise in complex multi-platform robotics integration, cross-language system architecture, and novel technology stacks. Focus on ROS2-based architectures integrating embedded systems, mobile platforms, and edge AI computing.

---

## [P013 - MRLink - VR Navigation & Data Collection Architecture with a Quadruped Robot]

<table class="content-table">
  <tr>
    <td width="55%">
This project was quite ambitious - developing a VR-integrated navigation system where AR glasses could control a Spot robot for autonomous data collection missions. What made this particularly challenging was creating a cross-platform architecture that could seamlessly connect Android devices, C# applications, and ROS2 systems.
      <br><br>
      The breakthrough was achieving the first successful Android + C# + ROS2 integration that enabled AR glasses control of robotic systems. I had to develop a custom ROS2 driver based on spot-sdk-cpp with Navigation2 integration, and modify rcldotnet for Android/Xamarin optimization to handle real-time data streaming.
      <br><br>
      For the edge computing, I distributed the AI workload across NVIDIA Jetson Xavier and Google Coral TPU architecture. The system integrated multi-sensor fusion with 3D LiDAR mapping and 360° cameras for environmental reconnaissance, real-time SLAM with VR operator oversight, and systematic mission planning for data gathering in complex environments.
      <br><br>
      The innovation here was pioneering the Android↔C#↔ROS2 architecture that enabled mobile VR devices as robot navigation control interfaces.
      <br><br>
      <strong>Videos:</strong> <a href="https://www.dropbox.com/scl/fi/w7hxeghhv6kutikgq73ho/2022.Meet-MRLINK-Spot.mp4?rlkey=1xfdkpo8yqumao0iqwy9mvl0a&dl=0">Meet MRLink</a> · <a href="https://www.dropbox.com/scl/fi/gt250oqa9yqcopjjuwk9u/video-holorobot-features-linkedin.mp4?rlkey=rurx22xzqismvjt4hdy8rosvu&dl=0">HoloRobot Features</a>
      <br><br>
      <a href="https://www.linkedin.com/posts/pabloinigoblasco_in-the-last-few-months-i-had-the-opportunity-activity-7103189317027586048-f-89">Technical Architecture</a> · <a href="https://www.linkedin.com/posts/qmartinez_mrlink-in-neurondones-activity-7321147566786531328-ZLRL/">MRLink Post</a>
    </td>
    <td width="45%">
      <img src="assets/mrlink-combined.png" alt="MRLink VR Navigation Architecture" width="500px">
    </td>
  </tr>
</table>

---

## [P014 - NeuronDones - Hazardous Environment Teleoperation Architecture of a Quadruped Robot]

<table class="content-table">
  <tr>
    <td width="55%">
This project focused on creating an integrated manipulation system for hazardous environment operations, combining VR teleoperation with multi-robot coordination. The goal was enabling precise manipulation tasks in nuclear, chemical, and high-radiation environments where human presence would be dangerous.
      <br><br>
      The platform integration was quite complex: Boston Dynamics Spot + Kinova Gen3 arm + Allegro Hand V4, all controlled through an Evergine-based immersive VR interface with haptic feedback. I developed custom inverse kinematics solvers and control algorithms for ROS2, and implemented real-time force feedback to transmit tactile sensations to the VR operator.
      <br><br>
      For environmental assessment, I integrated Azure Kinect for thermal imaging and developed multi-modal sensing that fused thermal, depth, and tactile sensor data. The custom algorithms enabled symbiotic human-robot operation where the operator could feel what the robot was touching and seeing.
      <br><br>
      This was actually the first VR-based multi-robot manipulation system for hazardous environments with integrated haptic feedback.
      <br><br>
      <strong>Videos:</strong> <a href="assets/neuron_dones.mp4">Main Demo</a> · <a href="https://www.dropbox.com/scl/fi/4w2duihdmz7fjrueyl2rd/2024-04-17_09-38-06-demo2-neuron-dones-xarm.mkv?rlkey=cmun89u4gmdjq6rli5ngnw64e&dl=0">xArm Integration (WIP)</a>
      <br><br>
      <a href="https://www.linkedin.com/posts/jcanton_neurondones-evergine-ros2-activity-7389571943223517184-mHrK">Technical Demo</a>
    </td>
    <td width="45%">
      <img src="assets/neurondones-combined.png" alt="NeuronDones Manipulation Architecture" width="500px">
    </td>
  </tr>
</table>

---

## [P010 - Hierarchical State Machine Architecture: SMACC2 + Nav2 Mission Control](https://www.dropbox.com/scl/fi/3stscugoptervds65ujqx/Dance-Party-at-AWS-Warehouse-Demo-1-gLH37M3e4e0.mkv?rlkey=izwjhwlei878nc9i16lk7r1id&dl=0)

<table class="content-table">
  <tr>
    <td width="55%">
This project demonstrated how to orchestrate complex robot missions using hierarchical state machine architecture. Working with SMACC2 and Nav2, I created a system that could handle sophisticated behavior sequences like navigation, pure rotation, and trajectory undo operations.
      <br><br>
      The architecture used SMACC2-based hierarchical mission control to orchestrate Nav2 primitives, with custom behavior trees interfacing with Navigation2 planners. I implemented real-time path generation, execution monitoring, and rollback capabilities, along with complex behavior composition for mission sequencing.
      <br><br>
      The implementation included custom ROS2 action servers for synchronized motion primitives, state-based recovery behaviors with automatic error handling, and a real-time trajectory visualization and debugging framework. I also built a modular behavior library for reusable mission components.
      <br><br>
      This project also had significance in simulation where Gazebo Classic provided the testing environment for mission-level behavior validation. The innovation was demonstrating a scalable approach to complex multi-behavior robot missions using formal state machine architecture.
      <br><br>
      <strong>Videos:</strong> <a href="https://www.dropbox.com/scl/fi/3stscugoptervds65ujqx/Dance-Party-at-AWS-Warehouse-Demo-1-gLH37M3e4e0.mkv?rlkey=izwjhwlei878nc9i16lk7r1id&dl=0">Demo 1</a> · <a href="https://www.dropbox.com/scl/fi/uyq7pqbp2z6413pogawwn/Dance-Party-at-AWS-Warehouse-Demo-2-A3kmCQS_ww8.mkv?rlkey=z0cvx7nhpcy5i72in3wp221pg&dl=0">Demo 2</a> · <a href="https://www.dropbox.com/scl/fi/7tbyr3a04w4k7ntsshmfe/Dance-Party-at-AWS-Warehouse-Demo-3-_4QZdvdTptI.mkv?rlkey=bgahwp6m6sh453i4rs1a0wa2d&dl=0">Demo 3</a>
    </td>
    <td width="45%">
      <img src="assets/aws-warehouse-dance-demo.png" alt="SMACC2 Hierarchical Mission Architecture" width="500px">
    </td>
  </tr>
</table>

---

## [P015 - Mobile AI Platform Robotization](https://www.dropbox.com/scl/fi/gsraxx5vrmbiuamq136xk/2018.Smart-Car-out-18-024028-combined-mobile-ai-platform.mp4?rlkey=8pdyohek1dqzm4ptiyf3xj1im&dl=0)

<table class="content-table">
  <tr>
    <td width="55%">
This was a comprehensive project where I took a completely non-robotized mobile base and converted it into an autonomous AI-enabled platform. It involved everything from hardware integration to embedded systems development - essentially building a robot from the ground up.
      <br><br>
      The hardware work was extensive: integrating motor controllers with CAN/UART interfaces, adding encoders, stereo and mono cameras, and LiDAR sensors from scratch. I implemented real-time control loops, kinematic modeling, and built a multi-sensor fusion system for localization and navigation.
      <br><br>
      For the software side, I adapted the ROS2 Nav2 stack and TEB planner to work with the platform's specific constraints, implemented low-level motor control with safety envelopes, and developed mission execution capabilities for waypoint following and obstacle avoidance.
      <br><br>
      What made this rewarding was achieving a complete physical transformation from a non-robotized platform to an autonomous mobile robot with integrated AI navigation stack. This project also had significance in motion planning where Ackermann steering models and TEB planner adaptations were developed.
      <br><br>
      <a href="https://www.dropbox.com/scl/fi/gsraxx5vrmbiuamq136xk/2018.Smart-Car-out-18-024028-combined-mobile-ai-platform.mp4?rlkey=8pdyohek1dqzm4ptiyf3xj1im&dl=0">Watch Video</a>
    </td>
    <td width="45%">
      <img src="assets/mobile_ai_platform.png" alt="Mobile AI Platform Hardware Integration" width="500px">
    </td>
  </tr>
</table>

---