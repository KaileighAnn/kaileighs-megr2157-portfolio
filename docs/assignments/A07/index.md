
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


### Design I – FEA Setup

The original bracket from A06 was used for the first static simulation in SolidWorks. The geometry and material were kept unchanged to establish a baseline for comparison with later designs.

#### Preprocessing

1. Opened the original bracket model from A06.
2. Created a new static study in SolidWorks Simulation.
3. Verified the Aluminum 6061-T6 material.
4. Identified the support locations and applied loading.
5. Prepared the model for mesh validation.

#### Simulation Setup Screenshot

![FEA Setup](images/A07/design1-setup.png)

*Figure 2. Static study setup for the original bracket.*

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
