# Single-link-design-project
cpp project ASU | Single link design and optimiztion 

Project Overview:
The goal is to develop a C++ program that designs a one-link robot actuated by a DC motor. The project has two main tasks:

Stress Analysis and Link Dimension Optimization

Motor and Gearbox Selection Optimization

Part 1: Stress Analysis and Link Dimension Optimization
Objective:
Determine the safest dimensions of the robot link to handle weight, inertial forces, and angular acceleration.

Input:
Cross-section type (Rectangle or Circle).

Material selection (from a predefined database with properties like yield strength and density).

Initial dimensions (Width, Height, or Radius).

Link length, payload mass, and max angular acceleration.

Equations Used:
Link Mass Calculation: Based on the material's density and the shape (Rectangle or Circle).

Bending Moment Calculation: Includes forces like weight and inertial force.

Moment of Inertia Calculation: Depends on the cross-section type.

Maximum Stress: Calculated using bending stress formulas.

Optimization Process:
Start with initial dimensions.

Calculate link mass, bending moment, and stress.

Adjust dimensions until stress is below the yield strength.

Return optimized link dimensions, mass, and final stress.

Part 2: Motor and Gearbox Selection Optimization
Objective:
Select an optimal motor-gearbox combination based on required torque, speed, and the lowest cost function (weight, diameter, and width).

Input:
Lists of available motors and gearboxes, including their specifications (torque, speed, mass, dimensions).

User-defined cost function priority (minimize weight, diameter, or width).

Equations Used:
Required Torque: Based on the mass and acceleration of the link and payload.

Motor-Gearbox Output Torque: Motor torque, gearbox ratio, and efficiency.

Motor-Gearbox Output Speed: Motor speed and gearbox ratio.

Optimization Process:
Filter motor-gearbox pairs that meet the required torque and speed.

Calculate the cost function for each pair.

Display the best combination minimizing the cost function.

Final Output:
Optimized link dimensions.

Final mass and stress value of the link.

Optimal motor-gearbox combination based on cost and performance.
