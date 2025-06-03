
# 🤖 3-DOF Robotic Arm – URDF Simulation

This repository contains the URDF model of a 3 Degrees of Freedom (DOF) robotic arm designed for simulation and visualization in **ROS 2** using **RViz** and optionally **Gazebo**.

---

## 📁 Project Structure

```

.
├── urdf/
│   └── arm\_2d.urdf       # Main URDF file describing the robot
├── launch/
│   └── display.launch.py # ROS 2 launch file for RViz visualization
├── config/
│   └── rviz\_config.rviz  # (Optional) Saved RViz visualization settings
├── meshes/               # (Optional) STL/DAE files if used
└── README.md

````


## 🎯 Features

- 3 rotational (revolute) joints
- Clean and modular URDF structure
- Color-coded links and joints
- Realistic link shapes (cylinders, spheres, box base)
- Ready-to-launch with RViz in ROS 2
- Simulates a 3-link articulated robotic arm

---

## 🧠 Degrees of Freedom

| Joint Name           | Type       | Axis     | Description                    |
|----------------------|------------|----------|--------------------------------|
| `base_arm_1_joint`   | Continuous | Y-axis   | Rotates first arm segment      |
| `arm_1_arm_3_joint`  | Continuous | Z-axis   | Rotates second segment         |
| `arm_3_arm_2_joint`  | Continuous | Y-axis   | Rotates third segment          |

**Total: 3 DOF (Rotational)**


## 🚀 Launch Instructions

> ✅ Prerequisite: ROS 2 (tested on Humble/Foxy) installed and sourced.

### 1. Clone the Repository

```bash
cd ~/ros2_ws/src
git clone https://github.com/your-username/three-dof-robotic-arm.git
cd ..
colcon build
source install/setup.bash
````

### 2. Launch in RViz

```bash
ros2 launch three_dof_robotic_arm display.launch.py
```

---

## 🛠️ To Do

* [ ] Add Xacro version of URDF
* [ ] Add joint controllers for simulation
* [ ] Add Gazebo plugin support
* [ ] Create Rviz interactive markers
* [ ] Add inverse kinematics support using MoveIt

---

## 📸 Preview

>![image](https://github.com/user-attachments/assets/2a6e26be-1186-4423-8774-8f75310452ce)

>![image](https://github.com/user-attachments/assets/2ef535ff-e88c-4dd5-a7e8-0d6295d38920)


---

## 🤝 Contributing

Feel free to open issues, submit pull requests, or suggest improvements!

---

## 📬 Contact

* LinkedIn: [Krishna Patel](www.linkedin.com/in/krishna-patel-77b032345)
* Email: [krishna.r282005@gmail.com](mailto:krishna.r282005@gmail.com)

```


