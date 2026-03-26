# CoppeliaSim Industrial Robot Vision Sorting System

This project demonstrates an **industrial automation system** developed in CoppeliaSim, integrating a robotic arm, conveyor belt, and vision sensor for real-time object detection and sorting.

---

## 📌 Project Overview

The system simulates an automated production line where objects are transported via a conveyor belt, detected using a vision sensor, and sorted by a robotic manipulator based on color.

It combines robotics, computer vision, and automation principles to replicate a real-world industrial sorting system.

---

## ⚙️ System Components

### 🤖 Robotic Arm (Dobot)

* 4-DOF robotic manipulator
* Performs pick-and-place operations
* Uses motion planning with velocity, acceleration, and jerk control

### 📦 Conveyor Belt

* Moves objects continuously
* Stops automatically when an object is detected
* Controlled using custom data communication

### 👁️ Vision Sensor

* Detects object color (Red / Green)
* Processes RGB values in real time
* Triggers robot actions

### 🚁 Drone / Mobile Robot (if included in your scene)

* Provides aerial monitoring / navigation
* Enhances simulation realism

---

## 🧠 System Workflow

1. Conveyor belt moves objects forward
2. Vision sensor scans objects
3. Color detection:

   * 🟢 Green object detected
   * 🔴 Red object detected
4. Conveyor stops
5. Robot executes pick-and-place:

   * Picks object from conveyor
   * Places in correct bin (based on color)
6. Conveyor resumes operation

---

## 🤖 Key Features

* 🎯 Real-time object detection using vision sensor
* 🎨 Color-based classification (Red / Green)
* 🦾 Automated pick-and-place robot control
* 🔄 Conveyor belt synchronization
* ⚡ Event-driven communication between components
* 🧠 Intelligent system coordination using scripts

---

## 🧠 Technical Concepts

* Industrial automation systems
* Robot kinematics and motion control
* Vision-based object detection
* Sensor-actuator integration
* Coroutine-based control in CoppeliaSim
* Real-time simulation

---

## 🧩 Code Explanation

### 🦾 Robot Control Script

* Uses coroutine-based execution
* Moves robot between:

  * Home position
  * Pickup position
  * Drop positions (Red / Green bins)
* Controls suction gripper

### 👁️ Vision Sensor Script

* Processes RGB values from detected objects
* Identifies:

  * Green objects
  * Red objects
* Sends signal to robot controller

### 📦 Conveyor Control

* Moves objects at constant velocity
* Stops when object detected
* Resumes after sorting

---

## ▶️ How to Run

1. Open CoppeliaSim
2. Load the scene:

   ```
   scene/industrial_simulation.ttt
   ```
3. Click **Start Simulation**
4. Observe:

   * Object detection
   * Conveyor control
   * Robot sorting

## 📊 Learning Outcomes

* Understanding industrial robotic systems
* Integration of vision and motion control
* Real-time system coordination
* Simulation of automated production lines

---
