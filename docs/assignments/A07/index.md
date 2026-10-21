
# A07 – Bracket FEA

## Objective

The objective of this assignment is to use Finite Element Analysis (FEA) to evaluate and improve the bracket designed in A05 and modeled in A06. The bracket will be analyzed for stress, displacement, safety factor, and mass. Geometry changes will be made to improve strength, stiffness, and weight.

## Original Bracket Design

The original bracket was designed using strength and stiffness calculations in A05 and modeled parametrically in SolidWorks for A06. This model will serve as the starting point for the FEA simulations.

### Design Requirements

| Parameter | Value |
|---|---|
| Material | Aluminum 6061-T6 |
| Applied Load | 600 lbf |
| Total Strap Load | 1,200 lbf |
| Safety Factor | 4 |
| Yield Strength | 40,000 psi |
| Modulus of Elasticity | 10 × 10⁶ psi |
| Maximum Allowable Deflection | 0.005 in |
| Allowable Stress | 10,000 psi |

### Original Dimensions

| Feature | Dimension | Value |
|---|---|---|
| A | Diameter | 0.875 in |
| B | Thickness | 0.150 in |
| C | Width | 1.375 in |
| D | Thickness | 0.050 in |
| E | Thickness | 1.375 in |

### Original CAD Model

<img width="787" height="808" alt="image" src="https://github.com/user-attachments/assets/787dab7e-ce7a-4769-9f6d-3aafce24a03e" />

*Figure 1. Original bracket model from A06.*

## FEA Validation – Inner Loop

A static stress analysis will be performed in SolidWorks Simulation. Three mesh sizes will be compared to evaluate convergence within 7%.

### Simulation Setup

- **Study Type:** Static
- **Material:** Aluminum 6061-T6
- **Fixtures:** To be documented
- **Applied Forces:** To be documented
- **Mesh Sizes:** Coarse, Medium, Fine

### Mesh Convergence

| Mesh Size | Elements | Max Stress (psi) | Max Displacement (in) | Safety Factor |
|---|---|---|---|---|
| Coarse | — | — | — | — |
| Medium | — | — | — | — |
| Fine | — | — | — | — |

## Design Optimization – Outer Loop

Three bracket designs will be evaluated. Geometry changes will be made based on the FEA results to improve strength, stiffness, and mass.


### Design I – Original Bracket FEA

The original bracket from A06 was analyzed using SolidWorks Simulation to evaluate its stress, displacement, and factor of safety. The geometry was kept unchanged to establish a baseline for future design improvements.

#### Preprocessing

1. Opened the original bracket model from A06.
2. Created a new static study in SolidWorks Simulation.
3. Assigned Aluminum 6061-T6 as the material.
4. Applied fixed geometry to two interior mounting faces.
5. Applied a 1,200 lbf downward load to the cylindrical feature.
6. Generated a high-quality solid mesh.
7. Ran the simulation to evaluate stress, displacement, and factor of safety.

#### Simulation Setup

- **Study Type:** Static
- **Material:** Aluminum 6061-T6
- **Applied Load:** 1,200 lbf downward
- **Fixtures:** Two interior mounting faces
- **Mesh Type:** High-quality solid mesh
- **Elements:** 1,280
- **Nodes:** 2,367
- **Failure Criterion:** Maximum von Mises Stress

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/6e6a013c-c837-43bf-bd96-af4c5844adf4" />

*Figure 2. Static simulation setup showing the applied load and fixed supports.*

#### Mesh Generation

A high-quality solid mesh was generated to divide the bracket into smaller elements for FEA calculations.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/fbc20111-2c64-4bd1-a912-fd7868640f5e" />

*Figure 3. Initial mesh generated for Design I.*

#### Stress Analysis

The maximum von Mises stress was approximately 396,000 psi, exceeding the material yield strength of 40,000 psi. The highest stresses occurred near the narrow vertical connection between the bracket and cylindrical feature.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/20b2dcfc-6f1b-4168-a376-3560f4292815" />

*Figure 4. Von Mises stress distribution for Design I.*

#### Displacement Analysis

The maximum resultant displacement was 28.72 mm (1.131 in), exceeding the allowable displacement of 0.005 in. The largest displacement occurred near the cylindrical feature.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/58f59ed7-81af-44d8-aaae-4075831e03fe" />

*Figure 5. Resultant displacement distribution for Design I.*

#### Factor of Safety

The minimum factor of safety was approximately 0.10, which is below the required safety factor of 4.0.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/560514fe-59ea-4808-9feb-c281500d3b83" />

*Figure 6. Factor of safety distribution for Design I.*

#### Initial FEA Results

| Measurement | Design I Result |
|---|---|
| Maximum von Mises Stress | 396,000 psi |
| Yield Strength | 40,000 psi |
| Maximum Displacement | 1.131 in |
| Allowable Displacement | 0.005 in |
| Minimum Factor of Safety | 0.10 |
| Required Factor of Safety | 4.0 |
| Number of Elements | 1,280 |
| Number of Nodes | 2,367 |

#### Design I Analysis

The initial simulation predicted stresses and displacement significantly exceeding the design requirements. The narrow vertical section experienced substantial bending under the applied load.

SolidWorks reported excessive displacement during the simulation. Because the predicted stress exceeds the yield strength, the linear static results are preliminary and require validation of the boundary conditions and mesh convergence.

The results identify the vertical connection as an important area to investigate when improving the bracket geometry.


### Design II – First Modification

To be completed after Design I.

### Design III – Second Modification

To be completed after Design II.

## Final Results

| Measurement | Design I | Design II | Design III |
|---|---|---|---|
| Maximum Stress and Location | — | — | — |
| Maximum Deflection and Location | — | — | — |
| Mass | — | — | — |
| Safety Factor | — | — | — |
| Number of Elements | — | — | — |

## Lessons Learned

To be completed after completing the FEA simulations.

## Time Spent

| Activity | Time |
|---|---|
| FEA Setup | — |
| Mesh Validation | — |
| Design Optimization | — |
| Documentation | — |
| **Total** | **—** |

## 2157 Students Only – Link FEA

The link developed in A05 and modeled in A06 will also be analyzed using FEA to evaluate its strength and stiffness.

### Original Link Dimensions

| Parameter | Value |
|---|---|
| Length | 3.00 in |
| Width | 1.50 in |
| Thickness | 0.25 in |
| Top Hole Diameter | 1.00 in |
| Bottom Hole Diameter | 0.875 in |

### Link Simulation Results

To be completed after the bracket analysis.
