# 🧪 2D Collision Simulator with Python

This project is an interactive simulator that represents collisions between particles in two dimensions using classical physics. It is designed for educational purposes, to facilitate the understanding of concepts such as momentum, mass, velocity, and elastic collisions.

---

## 🎯 Project Objective

Create a visual tool that allows:

- Configuring particles (position, mass, velocity, and color).
- Simulating their movements and collisions.
- Visualizing the results using the `pygame` graphics library.

---

## 📌 Features

- Support for multiple particles.
- Real-time motion visualization.
- Elastic collision calculations based on mass and direction.
- Graphical interface with `pygame_gui` to change parameters.

---

## 🖼️ Preview

Flow Diagram:
https://github.com/DannyLopezC/Proyecto_PDC/blob/main/diagrams/mainDiagram.drawio.png

---

## 🔧 Requirements

This project requires Python 3.8 or higher. The required dependencies are:

pip install pygame-ce pygame_gui numpy

If the pygame library is already installed, you must uninstall pygame and pygame-ce and then reinstall pygame-ce to avoid conflicts.

pip uninstall pygame-ce pygame

pip install pygame-ce

---

## ▶️ How to run the project

1. Clone this repository:

git clone https://github.com/DannyLopezC/Proyecto_PDC.git
cd Proyecto_PDC

2. Run the main file:

python main.py

This will open the simulator window with the particles in motion.

---

## 📁 Project Structure

Proyecto_PDC/
├── main.py # Main script
├── simulation.py # Collision and motion physics logic
├── visualization.py # Rendering particles on screen
├── interface_gui.py # Interface using pygame_gui
├── interface.py # Console parameters, currently obsolete
├── utils.py # Constants and helper functions
└── README.md # This file

---

## 🧠 Concepts Used

- 2D kinematics
- Conservation of linear momentum
- Elastic collisions
- Vectors with `numpy`

---

## 📸 Visual Example

Simulation:
https://github.com/DannyLopezC/Proyecto_PDC/blob/main/example.gif

---

## 📚 Credits

Project developed as a final programming alternative for the course **Computer Programming** at the National University of Colombia.

Author:
https://github.com/DannyLopezC
