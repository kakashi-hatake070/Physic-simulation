# Physic-simulation
Real-time cloth physics simulation built using Python and Pygame. Implements Verlet Integration and constraint-based spring mechanics to simulate soft-body behavior. Includes interactive drag and tear functionality with smooth 60 FPS rendering. Built from scratch to understand how physics engines work behind the scenes.

Cloth Physics Simulation using Python & Pygame
This project is a real-time cloth physics simulation built using Python and Pygame. The goal of this project was to understand how physics engines work internally and to implement a soft-body simulation system from scratch without using any external physics libraries.
The simulation is based on Verlet Integration, a technique commonly used in modern physics engines for stable and realistic motion. Instead of calculating velocity directly, the system updates positions using current and previous coordinates, resulting in smooth and natural cloth behavior. This approach provides better stability compared to traditional Euler integration methods.
The cloth is represented as a grid of interconnected points. Each point stores its current position, previous position, and a fixed state. The top row of points is pinned to simulate a hanging cloth. The connections between points act like springs using constraint satisfaction logic to maintain a constant distance between them. Multiple constraint-solving iterations are performed per frame to improve stability and realism.
The simulation runs at 60 FPS and includes real-time interactivity. Users can drag parts of the cloth using the left mouse button, creating dynamic movement and deformation. The right mouse button allows tearing of the cloth by removing constraints between points, making the simulation more engaging and realistic.
Key features include:
Verlet Integration for motion calculation
Constraint-based spring connections
Interactive drag and tear mechanics
Gravity simulation
Real-time rendering using Pygame
This project helped deepen my understanding of physics simulations, mathematical modeling, constraint solving, and real-time graphics rendering. It demonstrates how mathematical concepts translate into interactive visual systems.
Future improvements may include adding wind forces, collision detection, texture mapping, and converting the simulation into a flag or soft-body game mechanic.
Built with Python and a strong curiosity to understand how game physics works behind the scenes.
