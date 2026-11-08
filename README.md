# maze-solver-robot
#An autonomous maze-solving robot developed using the Teensy 4.1 microcontroller, designed to explore and navigate a 16×16 maze using the Flood Fill Algorithm. The system integrates IR-based wall detection, Time-of-Flight distance sensing, motor encoder feedback and gyroscope-based motion sensing for autonomous navigation and shortest-path calculation.
#**Project Overview**
#The Maze Solver Robot is an embedded robotics project focused on autonomous maze exploration and pathfinding. It detects walls, maintains maze information, calculates optimal paths using the Flood Fill algorithm and navigates towards the destination.
#**The robot follows a two-stage approach:**
#Exploration Phase: Explores the maze and identifies walls and accessible paths.
#Shortest Path Phase: Calculates and follows the optimal route towards the destination using updated maze information.
#**Key Features**
#Autonomous navigation through a 16×16 maze.
#Flood Fill algorithm for maze exploration and shortest-path calculation.
#IR sensor-based wall detection.
#VL53L0X Time-of-Flight distance measurement.
#Motor encoder feedback for movement control.
#6-axis gyroscope for motion sensing.
#Dual N20 DC motor control.
#Teensy 4.1-based embedded control architecture.
#**Hardware Components**
🧠 Working Principle

1. Maze Exploration

The robot moves through the maze and detects surrounding walls using four TCRT5000 IR sensors.

2. Distance Measurement

The VL53L0X ToF sensor provides distance measurements to assist navigation.

3. Maze Mapping

Detected walls and accessible paths are used to maintain the internal representation of the maze.

4. Flood Fill Algorithm

The algorithm assigns distance values to maze cells and repeatedly updates them according to accessible neighboring cells.

5. Path Selection

The robot selects an accessible neighboring cell with the lowest distance value to move towards the destination.

6. Shortest Path Navigation

After exploration, the robot uses the calculated distance map to follow an optimal route towards the destination.

🧮 Algorithm – Flood Fill

The Flood Fill algorithm is a pathfinding technique commonly used in maze-solving robots.

Algorithm Workflow:

Initialize the maze and distance values.

Assign the destination cell a distance value of zero.

Update the distance values of neighboring cells.

Consider wall information to determine accessible paths.

Select the neighboring cell with the lowest distance value.

Repeat distance updates whenever required.

Navigate towards the destination using the calculated path.

📁 Repository Structure

maze-solver-robot/
│
├── README.md
│
├── firmware/
│   └── maze_solver/
│
├── hardware/
│   ├── circuit_diagrams/
│   ├── pcb_design/
│   └── pinout/
│
├── documentation/
│   ├── working_principle.md
│   ├── flood_fill_algorithm.md
│   └── components_list.md
│
└── images/
    ├── robot/
    └── testing/

📷 Project Gallery

Project photographs, hardware assembly, circuit diagrams and testing demonstrations are included in the repository.

🎯 Applications

Autonomous mobile robotics.

Maze exploration and pathfinding.

Embedded systems and firmware development.

Sensor integration and motor control.

Robotics navigation algorithms.

👨‍💻 Developer

Viral Parekh

Electronics & Communication Engineering

GitHub: viralkparekh

LinkedIn: Viral Parekh
