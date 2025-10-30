# MAT-350 Project 1: Network Flow Analysis Using Linear Systems

**Author:** Justin Paul Guida  
**Course:** MAT-350 - Applied Linear Algebra  
**Date:** September 18, 2025  


## Overview
This project models a **computer network flow system** using **systems of linear equations**.  
Each router in the network (A, B, C, D, and E) is represented as a node, and data transfer between routers is modeled using equations that balance inflow and outflow rates.

The project demonstrates how to construct a coefficient matrix `A`, a constant vector `b`, and solve the system `Ax = b` using MATLAB.  
It also includes validation through **LU decomposition**, **Cramer’s Rule**, and determinant analysis.

The project is submitted as a report (`.pdf`) generated in MATLAB, showing full calculations, code, and annotated results.



## Objectives
1. Develop a linear system of equations for a five-router network.  
2. Represent the system in matrix form (`Ax = b`).  
3. Solve the system using MATLAB’s built-in tools (`rref`, `lu`, `inv`, `det`).  
4. Verify the solution using multiple algebraic methods.  
5. Interpret network flow results and identify potential system bottlenecks or upgrade recommendations.


## Key MATLAB Concepts Demonstrated
- **Matrix Construction:** Defining coefficient matrices and augmented matrices.  
- **Row Reduction:** Solving systems using `rref()` for reduced row echelon form.  
- **LU Decomposition:** Breaking down `A` into lower (`L`) and upper (`U`) matrices.  
- **Forward/Backward Substitution:** Solving `Ly = b` and `Ux = y`.  
- **Matrix Inversion:** Using `inv()` to compute the inverse of `U`.  
- **Determinants and Cramer’s Rule:** Cross-verifying results using determinant calculations.



## Results Summary
- All routers yield unique flow values with no free variables, confirming a consistent system.  
- The final data flow vector was determined to be:

x = [50; 25; 30; 100; 45] Mbps

- Determinant of the system matrix `A` is **2.00**, confirming the system’s invertibility.  
- LU and Cramer’s Rule methods both reproduce identical results.  
- Network recommendations include upgrading links nearing capacity to prevent congestion.



## File Description
| File | Description |
|------|--------------|
| `mat350_project1_network_flow_analysis.pdf` | Final report with MATLAB code, output, and written explanations. |



## Tools and Requirements
- MATLAB R2023a or later  
- No additional toolboxes required  


## Educational Purpose
This project reinforces the application of **linear algebra in network modeling**, demonstrating how fundamental matrix operations can represent and analyze real-world data flow systems.  
It highlights the practical use of MATLAB for solving and verifying linear systems in engineering and applied mathematics contexts.

