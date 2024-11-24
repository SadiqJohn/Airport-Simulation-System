# Airport Simulation System

This project is an **Airport Simulation System** developed as a part of an intermediate C programming course. The simulation models an airport's operations, including plane creation, prioritization, and monitoring of fuel levels, statuses, and outcomes (landed or crashed). The system also allows user interaction to control the simulation and check the status of planes dynamically.

---

## Features

### 1. Priority-Based Plane Queue
- Planes are queued based on their priority:
  - **Air Force 1:** Highest priority.
  - **Private Planes:** Medium priority.
  - **Commercial Planes:** Lowest priority.
- Emergency scenarios automatically re-prioritize planes with low fuel.

### 2. Status Tracking
- Planes can have the following statuses:
  - **QUEUED:** Waiting in the priority queue.
  - **CIRCLING:** Active in simulation, consuming fuel.
  - **LANDING NEXT:** Highest priority plane about to land.
  - **LANDED:** Successfully landed planes stored in a stack.
  - **CRASHED:** Planes that ran out of fuel stored in a crash stack.

### 3. Real-Time Simulation
- Dynamic simulation loop:
  - Reduces plane fuel by 5% per cycle.
  - Updates plane statuses and priorities based on conditions.
  - Handles landings or crashes at each iteration.

### 4. User Interaction
- Interactive console menu:
  - **Create a new plane.**
  - **Simulate one cycle or full simulation.**
  - **Check the status of planes.**
  - **View landed or crashed planes.**
  - **Quit the simulation.**

### 5. Randomized Plane Initialization
- New planes are assigned a random initial fuel level between 10% and 90%.

---

## Concepts Demonstrated

This project demonstrates the following programming skills and concepts:

- **Object-Oriented Programming (OOP):** 
  - Classes for encapsulating data and behaviors (`Plane`, `Airport`).
- **Data Structures:**
  - **Queues:** Priority-based linked list for managing active planes.
  - **Stacks:** Efficient storage and retrieval of landed and crashed planes.
- **Dynamic Memory Management:** 
  - Use of pointers for memory allocation and deallocation.
- **Control Flow:**
  - Logic for prioritization, status updates, and emergency handling.
- **Algorithm Design:** 
  - Sorting planes dynamically based on priority.
- **Standard Library Usage:** 
  - Libraries like `<iostream>`, `<iomanip>`, and `<sstream>` for input/output formatting.

---

## How to Use

### Prerequisites
- A C++ compiler (e.g., GCC, Clang, or Visual Studio).
- Basic knowledge of C++ and object-oriented programming.

### Compilation and Execution
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/airport-simulation.git
   cd airport-simulation
