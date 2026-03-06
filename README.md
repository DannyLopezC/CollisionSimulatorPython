# 🧪 2D Collision Simulator with Python

This project is an interactive simulator that represents collisions
between particles in two dimensions using classical physics. It is
designed for educational purposes, to facilitate the understanding of
concepts such as momentum, mass, velocity, and elastic collisions.

------------------------------------------------------------------------

## 🎯 Project Objective

Create a visual tool that allows:

-   Configuring particles (position, mass, velocity, and color).
-   Simulating their movements and collisions.
-   Visualizing the results using the `pygame` graphics library.

------------------------------------------------------------------------

## 📌 Features

-   Support for multiple particles.
-   Real-time motion visualization.
-   Elastic collision calculations based on mass and direction.
-   Graphical interface with `pygame_gui` to change parameters.

------------------------------------------------------------------------

## 🖼️ Preview

![Flow
Diagram](https://github.com/DannyLopezC/CollisionSimulatorPython/blob/main/diagrams/mainDiagram.drawio.png)

------------------------------------------------------------------------

## 🔧 Requirements

This project requires Python 3.8 or higher. The required dependencies
are:

pip install pygame-ce pygame_gui numpy

If the pygame library is already installed, you must uninstall pygame
and pygame-ce and then reinstall pygame-ce to avoid conflicts.

pip uninstall pygame-ce pygame pip install pygame-ce

------------------------------------------------------------------------

## ▶️ How to run the project

1.  Clone this repository:

git clone https://github.com/DannyLopezC/CollisionSimulatorPython.git cd
CollisionSimulatorPython

2.  Run the main file:

python main.py

This will open the simulator window with the particles in motion.

------------------------------------------------------------------------

## 📁 Project Structure

CollisionSimulatorPython/ ├── main.py \# Main application entry point
├── simulation.py \# Physics logic for collisions and motion ├──
visualization.py \# Rendering of particles on screen ├──
interface_gui.py \# Graphical interface using pygame_gui ├──
interface.py \# Console parameter interface (currently unused) ├──
utils.py \# Constants and helper functions └── README.md \# Project
documentation

------------------------------------------------------------------------

## 🧠 Concepts Used

-   2D kinematics
-   Conservation of linear momentum
-   Elastic collisions
-   Vector operations with `numpy`

------------------------------------------------------------------------

## 📸 Visual Example

![Simulation](https://github.com/DannyLopezC/CollisionSimulatorPython/blob/main/example.gif)

------------------------------------------------------------------------

## 🏗 Architecture

The simulator follows a modular architecture that separates the physics
model, visualization, and user interaction. This structure improves
readability, maintainability, and extensibility of the code.

### Simulation Core

The **simulation module** contains the core physics logic responsible
for particle behavior.

Responsibilities include:

-   Updating particle positions over time
-   Detecting collisions between particles
-   Resolving elastic collisions using conservation of momentum
-   Managing physical properties such as mass and velocity

This module operates independently from any graphical interface,
allowing the physics model to remain clean and reusable.

------------------------------------------------------------------------

### Visualization Layer

The **visualization module** handles rendering using `pygame`.

Responsibilities include:

-   Drawing particles on screen
-   Updating the simulation frame
-   Converting simulation coordinates into screen coordinates

The visualization layer does not contain physics calculations and simply
represents the current state of the simulation.

------------------------------------------------------------------------

### Interface Layer

User interaction is handled through interface modules.

Two interaction approaches exist in the project:

-   **Graphical interface (`interface_gui.py`)** built with `pygame_gui`
-   **Console interface (`interface.py`)**, originally used for
    parameter configuration

The graphical interface allows users to modify simulation parameters
such as particle mass, velocity, and initial position.

------------------------------------------------------------------------

### Main Controller

The `main.py` file acts as the **application controller**, coordinating
the interaction between modules.

Its responsibilities include:

-   Initializing the simulation
-   Updating the physics state
-   Rendering the visualization
-   Processing user input

This central control loop ensures that simulation updates, rendering,
and user interaction remain synchronized.

------------------------------------------------------------------------

### Utilities Module

The `utils.py` module contains shared constants and helper functions
used throughout the project.

Examples include:

-   Physical constants
-   Vector helper functions
-   Shared configuration values

Centralizing these elements prevents duplication and keeps the main
modules focused on their core responsibilities.

------------------------------------------------------------------------

## 📚 Credits

Project developed as a final programming alternative for the course
**Computer Programming** at the National University of Colombia.

Author: [DannyLopezC](https://github.com/DannyLopezC)
