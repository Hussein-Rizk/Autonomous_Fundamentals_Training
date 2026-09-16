# 🚗 Autonomous Fundamentals Training — 2023

**Mansoura Motorsport — Mansoura University**

A **20-hour training course in Autonomous Fundamentals** completed in 2023 at the Faculty of Engineering, Mansoura University.

The training introduced the main building blocks of an autonomous vehicle, progressing from the fundamentals of self-driving systems to **perception, sensor fusion, SLAM, motion planning, simulation, ROS, and vehicle control**.

---

## 🎓 Certificate

<p align="center">
  <a href="./Autonomous%20Fundamentals%20Training%20Certificate.pdf">
    <img src="./Autonomous%20Fundamentals%20Training%20Certificate.png"
         alt="Autonomous Fundamentals Training Certificate"
         width="80%">
  </a>
</p>

<p align="center">
  <b>Click the certificate to view the original PDF.</b>
</p>

**Training Duration:** 20 Hours  
**Dates:** 23 September – 10 October 2023  
**Organization:** Mansoura Motorsport  
**Location:** Faculty of Engineering, Mansoura University  

---

# 📚 Training Content

The repository contains the original material from **seven training sessions** covering the major components of an autonomous-vehicle system.

```text
Autonomous Vehicle Fundamentals
            ↓
     Sensors & Perception
            ↓
Computer Vision & Sensor Fusion
            ↓
            SLAM
            ↓
      Motion Planning
            ↓
     Simulation & ROS
            ↓
       Control Theory
```

---

## 1️⃣ Introduction to Autonomous Vehicles

The first session introduces autonomous vehicles and the overall self-driving problem.

Topics include:

- Definition of autonomous systems and robots
- History and development of autonomous vehicles
- Applications of autonomous robotics
- Autonomous-vehicle racing competitions
- Motivation for autonomous driving
- Driving-task decomposition
- Perception
- Motion planning
- Vehicle control
- Lateral and longitudinal control
- Object and Event Detection and Response (**OEDR**)
- Levels of driving automation
- Challenges facing autonomous vehicles
- Legal and ethical considerations

The session presents the autonomous-driving task as three major components:

```text
Perception
    ↓
Motion Planning
    ↓
Vehicle Control
```

---

## 2️⃣ Autonomous Vehicle Systems & Sensors

The second session focuses on how an autonomous vehicle gathers information from its environment and uses that information for decision-making.

### Sensors Introduced

- LiDAR
- Radar
- Camera
- Stereo camera
- IMU
- Accelerometer
- Gyroscope
- Magnetometer
- GNSS

The session also discusses the difference between **active and passive sensing**.

### Perception Goals

The vehicle must be able to identify:

- Static objects
- Dynamic objects
- Pedestrians
- Vehicles
- Bicycles and motorcycles
- Road signs
- Traffic lights
- Road boundaries

It also introduces **ego-localization**, including estimation of position, velocity, acceleration, orientation, and angular motion.

### Planning Concepts

Decision-making is discussed at several levels:

- Long-term / mission planning
- Short-term planning
- Immediate / trajectory planning
- Rule-based planning
- Predictive planning

---

## 3️⃣ Perception, Computer Vision & Sensor Fusion

The third session explores how computers interpret the environment surrounding an autonomous vehicle.

### Information Required

A self-driving system may need to determine:

- Pedestrian locations
- Nearby vehicles
- Traffic signs
- Drivable space
- Curbs
- Lane positions

### Computer Vision Pipeline

```text
Image Input
    ↓
Preprocessing
    ↓
Feature Detection
    ↓
Feature Description
    ↓
Feature Matching
    ↓
Environment Understanding
```

Topics introduced include:

- Image preprocessing
- Histogram equalization
- Color correction
- Noise removal
- Feature extraction
- Feature detection
- Feature descriptors
- Feature matching
- Neural networks
- Convolutional Neural Networks (**CNNs**)

### Sensor Fusion

The session emphasizes combining information from multiple sensors such as cameras, LiDAR, IMU, and GPS/GNSS to improve accuracy, reliability, coverage, robustness, and state estimation.

---

## 4️⃣ SLAM — Simultaneous Localization and Mapping

The fourth session introduces **SLAM**, one of the core technologies used in autonomous robotics.

SLAM enables a robot to:

> **Build a map of an environment while simultaneously estimating its own position inside that map.**

### SLAM Workflow

```text
Data Acquisition
       ↓
Feature Extraction
       ↓
Sensor Fusion
       ↓
Mapping
       ↓
Localization
       ↓
Loop Closure
       ↓
Optimization
```

### Map Representations

- Occupancy Grid Maps
- Point Cloud Maps
- Feature-Based Maps

### Localization

Topics include:

- Global localization
- Local localization
- Particle filters
- Monte Carlo Localization
- Kalman Filters
- Extended Kalman Filters
- Iterative Closest Point

### Loop Closure & Optimization

Introduced concepts include:

- Loop-closure detection
- Loop constraints
- Graph representation
- Graph-based optimization
- Bundle adjustment
- Nonlinear optimization

### SLAM Algorithms Introduced

- EKF-SLAM
- FastSLAM
- Graph-Based SLAM
- ORB-SLAM
- Hector SLAM
- Google Cartographer
- LiDAR-based SLAM
- LSD-SLAM

The session also discusses selecting SLAM algorithms based on sensors, computational resources, environment complexity, real-time requirements, cost, and robustness.

---

## 5️⃣ Motion Planning

The fifth session focuses on how an autonomous vehicle decides **how to move safely from a starting position to a destination**.

### Fundamental Concepts

- Configuration space
- State space
- Degrees of Freedom (**DOF**)
- Path vs. trajectory
- Occupancy grids
- Graph representation

### Path vs. Trajectory

A **path** describes where the vehicle should move geometrically, while a **trajectory** adds time, velocity, and dynamic-state information.

### Planning Hierarchy

```text
Mission Planning
      ↓
Behavior Planning
      ↓
Local Planning
```

### Mission Planning

Graph-search methods introduced include:

- **Dijkstra's Algorithm**
- **A\* Algorithm**

The session discusses directed and undirected graphs, weighted graphs, shortest-path search, cost functions, heuristics, and algorithm optimization.

### Behavior Planning

Introduced approaches include:

- Finite State Machines (**FSM**)
- Rule-based systems
- Reinforcement-learning concepts

### Local Planning

Local planning focuses on generating feasible, collision-free paths and comfortable velocity profiles. The session also introduces **sampling-based planning** and **Rapidly-exploring Random Trees (RRT)**.

---

## 6️⃣ Autonomous-System Simulation & ROS

The sixth session introduces simulation as a development and testing tool for autonomous systems.

### Why Simulation?

Simulation can provide:

- Cost reduction
- Reproducibility
- Scalability
- Rapid prototyping
- Safe testing
- Data collection
- Unlimited testing environments
- Reduced risk of physical damage

### Simulation Types

#### Hardware-in-the-Loop (HIL)

Combines real hardware with a simulated environment.

Example tools mentioned:

- dSPACE
- NI VeriStand
- OPAL-RT

#### Sensor Simulation

Used to simulate sensors such as LiDAR, radar, and cameras.

Example environments discussed include:

- ROS / Gazebo
- Autoware
- MATLAB / Simulink

#### Scenario Simulation

Used to reproduce driving situations such as lane changes, intersections, and emergency situations.

Example platforms introduced:

- CARLA
- NVIDIA DRIVE Sim
- LGSVL

### 🤖 ROS Fundamentals

The simulation session also introduces the **Robot Operating System (ROS)**.

Topics include:

- Hardware abstraction
- ROS filesystem
- Libraries and tools
- Message passing
- Nodes
- Topics
- Messages
- Services
- Actions
- Parameter Server
- ROS Bags
- `roscore`
- Catkin
- ROS workspaces
- ROS packages

The material also introduces creation of a Catkin workspace and the basic **publisher / subscriber communication model**.

```text
ROS Master
    ↓
Publisher Node
    ↓
   Topic
    ↓
Subscriber Node
```

---

## 7️⃣ Control Theory & PID Control

The final session connects autonomous-system decision making with actual vehicle control.

### Control-System Fundamentals

The training compares:

- Open-loop control
- Closed-loop control

A closed-loop system uses sensor feedback to compare the desired state with the actual system state.

### PID Controller

The session introduces the three PID components:

- **P — Proportional**
- **I — Integral**
- **D — Derivative**

and their influence on characteristics such as:

- Rise time
- Overshoot
- Settling time
- Steady-state error
- Stability

### PID Issues

The material also introduces common practical issues including:

- Measurement noise
- Low-pass filtering
- Integral wind-up
- Clamping
- Back-calculation
- Observer-based approaches

---

# 🧠 Autonomous-System Architecture

Across the seven sessions, the training presents autonomous driving as an integrated system:

```text
                    Sensors
                      │
       ┌──────────────┼──────────────┐
       │              │              │
     Camera          LiDAR        Radar / IMU
       │              │              │
       └──────────────┼──────────────┘
                      ▼
                 Perception
                      │
                      ▼
               Sensor Fusion
                      │
                      ▼
             Localization / SLAM
                      │
                      ▼
               Motion Planning
                      │
                      ▼
                Vehicle Control
                      │
                      ▼
           Steering / Brake / Throttle
```

---

# 🛠️ Technologies & Concepts Introduced

### Autonomous Systems
- Autonomous vehicles
- OEDR
- Driving automation levels
- Ego-localization

### Sensors
- Camera
- Stereo vision
- LiDAR
- Radar
- IMU
- GNSS

### Computer Vision
- Image preprocessing
- Feature detection
- Feature description
- Feature matching
- CNN concepts

### Localization & Mapping
- SLAM
- Occupancy grids
- Point clouds
- EKF
- Particle filters
- Graph optimization
- Loop closure

### Planning
- Dijkstra
- A*
- RRT
- Finite State Machines
- Rule-based planning
- Mission / behavior / local planning

### Simulation & Robotics
- ROS
- Catkin
- Nodes
- Topics
- Publisher / Subscriber
- HIL simulation
- Sensor simulation
- Scenario simulation

### Control
- Open-loop control
- Closed-loop control
- PID control


---

# 🎯 What This Training Demonstrates

The training provided foundational exposure to:

- Autonomous-vehicle architecture
- Robotics fundamentals
- Autonomous-driving sensors
- Computer vision
- Sensor fusion
- Localization
- SLAM
- Mapping
- Motion planning
- Graph-search algorithms
- Simulation
- ROS architecture
- Control systems
- PID control

It helped establish the relationship between the major subsystems required to create an autonomous robot or vehicle:

> **Sense → Perceive → Localize → Plan → Control**

---

## 📌 Training Information

**Training:** Autonomous Fundamentals  
**Organization:** Mansoura Motorsport  
**Institution:** Faculty of Engineering — Mansoura University  
**Duration:** 20 Hours  
**Dates:** 23 September – 10 October 2023  
**Year:** 2023

> Foundational autonomous-systems training covering perception, localization, mapping, planning, simulation, ROS, and vehicle control.
