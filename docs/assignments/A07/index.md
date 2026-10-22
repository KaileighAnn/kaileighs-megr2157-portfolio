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

The original bracket from A06 was analyzed using SolidWorks Simulation to evaluate its stress, displacement, and factor of safety. The geometry remained unchanged to establish a baseline for future design improvements.

#### Preprocessing

1. Opened the original bracket model from A06 in SolidWorks.
2. Created a static study using SolidWorks Simulation.
3. Assigned Aluminum 6061-T6 as the material.
4. Applied fixed geometry to two interior mounting faces.
5. Applied a 600 lbf downward load to the cylindrical feature.
6. Generated high-quality solid meshes at three different densities.
7. Ran each simulation to evaluate stress, displacement, and factor of safety.
8. Compared the results to evaluate mesh convergence.

#### Simulation Setup

| Parameter | Value |
|---|---|
| Study Type | Static |
| Material | Aluminum 6061-T6 |
| Applied Load | 600 lbf downward |
| Fixtures | Two interior mounting faces |
| Load Location | Cylindrical feature |
| Mesh Type | High-quality solid mesh |
| Failure Criterion | Maximum von Mises Stress |
| Yield Strength | 40,000 psi |
| Required Safety Factor | 4.0 |
| Maximum Allowable Displacement | 0.005 in |

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/de2754ab-a2a6-425b-851a-f631fbc70664" />

*Figure 2. Static simulation setup showing the 600 lbf downward load and fixed mounting faces.*

#### Mesh Generation

Three different mesh densities were evaluated to determine the effect of element size on the FEA results.

The coarse mesh was used for the initial analysis. The mesh was then refined to improve the accuracy of the calculated stress and displacement.

The refined mesh used high-quality solid elements to better represent the bracket geometry.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/1bacbc28-7311-4ebe-a352-5b6eeb12dd8d" />

*Figure 3. High-quality solid mesh generated for Design I.*

#### Mesh Convergence Results

| Mesh Size | Maximum Stress (psi) | Maximum Displacement (in) | Minimum Safety Factor |
|---|---|---|---|
| Coarse | 164,600 | 0.426 | 0.24 |
| Fine | 220,500 | 0.601 | 0.18 |
| Refined | 240,900 | 0.618 | 0.17 |

The maximum stress and displacement increased as the mesh became finer. All three simulations predicted that the bracket exceeded the design requirements.

#### Coarse Mesh Analysis

The coarse mesh was used for the first simulation with the corrected 600 lbf load.

##### Von Mises Stress

The maximum von Mises stress was approximately 164,600 psi, exceeding the material yield strength of 40,000 psi.

The highest stresses occurred near the narrow vertical section connecting the upper bracket to the cylindrical feature.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/980fed47-a11a-4cb4-beab-0c7801131887" />

*Figure 4. Von Mises stress distribution for the coarse mesh.*

##### Displacement

The maximum resultant displacement was approximately 10.83 mm (0.426 in), exceeding the allowable displacement of 0.005 in.

The largest displacement occurred near the cylindrical feature.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/1627b81d-2119-4a66-ac67-7e5f9b2e1545" />

*Figure 5. Resultant displacement distribution for the coarse mesh.*

##### Factor of Safety

The minimum factor of safety was approximately 0.24, which is below the required safety factor of 4.0.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/42f62cef-0463-4833-8b65-bda81ac46d0f" />

*Figure 6. Factor of safety distribution for the coarse mesh.*

#### Fine Mesh Analysis

A finer mesh was generated to evaluate the effect of increased mesh density on the simulation results.

##### Von Mises Stress

The maximum von Mises stress increased to approximately 220,500 psi.

The highest stresses remained concentrated near the narrow vertical connection.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/542d8f1d-b1b3-4352-a4aa-f61ae383c483" />

*Figure 7. Von Mises stress distribution for the fine mesh.*

##### Displacement

The maximum resultant displacement increased to approximately 15.27 mm (0.601 in).

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/9290891d-ecf3-4f81-965b-d6316e40795d" />

*Figure 8. Resultant displacement distribution for the fine mesh.*

##### Factor of Safety

The minimum factor of safety decreased to approximately 0.18.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/971cb4e7-bee6-46c7-9015-8798813e2f21" />

*Figure 9. Factor of safety distribution for the fine mesh.*

#### Refined Mesh Analysis

A refined mesh was generated for the final comparison of Design I.

##### Von Mises Stress

The maximum von Mises stress was approximately 240,900 psi.

This value exceeded both the allowable stress of 10,000 psi and the material yield strength of 40,000 psi.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/bd4140d7-e8a9-47fa-8736-b08ae3353bd9" />

*Figure 10. Von Mises stress distribution for the refined mesh.*

##### Displacement

The maximum resultant displacement was approximately 15.69 mm (0.618 in).

This exceeded the maximum allowable displacement of 0.005 in.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/6b50123b-49db-4135-9f1f-0aba3c51eb75" />

*Figure 11. Resultant displacement distribution for the refined mesh.*

##### Factor of Safety

The minimum factor of safety was approximately 0.17, which is significantly below the required value of 4.0.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/a877d513-1a55-4c32-bb66-bfbc07d230c3" />

*Figure 12. Factor of safety distribution for the refined mesh.*

#### Mesh Convergence Evaluation

The fine and refined mesh results were compared to determine whether the simulation satisfied the 7% convergence requirement.

**Percentage Difference Formula:**

Percentage Difference = |Refined − Fine| / Refined × 100

**Stress Convergence**

Percentage Difference = |240,900 − 220,500| / 240,900 × 100

**Stress Difference = 8.47%**

**Displacement Convergence**

Percentage Difference = |0.618 − 0.601| / 0.618 × 100

**Displacement Difference = 2.75%**

| Measurement | Percentage Difference | Requirement | Result |
|---|---|---|---|
| Maximum Stress | 8.47% | Less than 7% | Not Met |
| Maximum Displacement | 2.75% | Less than 7% | Met |

The displacement results satisfied the 7% convergence requirement. However, the maximum stress results did not, indicating that further mesh refinement may be necessary.

#### Final Design I Results

| Measurement | Design I Result | Requirement | Status |
|---|---|---|---|
| Maximum von Mises Stress | 240,900 psi | 10,000 psi allowable | Not Met |
| Maximum Displacement | 0.618 in | 0.005 in maximum | Not Met |
| Minimum Factor of Safety | 0.17 | 4.0 minimum | Not Met |
| Material | Aluminum 6061-T6 | Aluminum 6061-T6 | Met |
| Applied Load | 600 lbf | 600 lbf | Met |
| Stress Mesh Convergence | 8.47% | Less than 7% | Not Met |
| Displacement Mesh Convergence | 2.75% | Less than 7% | Met |

#### Design I Analysis

The FEA results showed that the original bracket did not meet the strength or stiffness requirements under the applied 600 lbf load.

The highest stresses occurred near the narrow vertical connection between the upper bracket and cylindrical feature. This section experienced substantial bending under the applied load.

The maximum displacement occurred near the cylindrical feature, indicating that the original geometry was not sufficiently stiff.

The refined mesh predicted a minimum factor of safety of approximately 0.17, which was significantly below the required value of 4.0.

Because the predicted stresses exceeded the material yield strength, the linear static results should be treated as preliminary rather than accurate predictions of permanent deformation. The stress results also require further mesh refinement to satisfy the convergence requirement.

#### Design I Conclusion

The original bracket did not satisfy the required stress, displacement, or factor of safety limits. Mesh refinement showed that displacement was approaching convergence, while stress convergence remained above the 7% requirement.

The narrow vertical connection was identified as a critical area for future design improvements. Additional analysis and geometry modifications will be investigated in Design II to improve the bracket's strength and stiffness.


#### Design I Analysis

The initial simulation predicted stresses and displacement significantly exceeding the design requirements. The narrow vertical section experienced substantial bending under the applied load.

SolidWorks reported excessive displacement during the simulation. Because the predicted stress exceeds the yield strength, the linear static results are preliminary and require validation of the boundary conditions and mesh convergence.

The results identify the vertical connection as an important area to investigate when improving the bracket geometry.



## Design 2 – Modified Bracket

### Design

Design 2 was developed as an improvement to Design 1 to increase the strength and stiffness of the bracket. The geometry was modified while maintaining a symmetrical design and the original mounting and loading features.

The updated model was created in SOLIDWORKS using Aluminum 6061-T6.

### Design Modifications

- Modified the bracket geometry to improve structural support.
- Maintained symmetry about the vertical centerline.
- Retained the upper mounting section and U-shaped opening.
- Retained the lower cylindrical loading feature.
- Preserved the original loading and mounting conditions for comparison with Design 1.

### Finite Element Analysis (FEA)

Three static studies were completed in SOLIDWORKS Simulation using coarse, fine, and refined meshes.

#### Simulation Settings

| Parameter | Value |
|---|---|
| Material | Aluminum 6061-T6 |
| Applied Load | 600 lbf |
| Load Direction | Downward |
| Fixture | Fixed geometry at two upper mounting faces |
| Yield Strength | 40,000 psi (approximately 275 MPa) |
| Required Factor of Safety | 4 |
| Maximum Allowable Displacement | 0.005 in |
| Analysis Type | Linear Static |
| Mesh Quality | High |
| Mesh Studies | Coarse, Fine, Refined |

### FEA Results

| Mesh | Maximum von Mises Stress (MPa) | Maximum Displacement (mm) | Minimum FOS |
|---|---:|---:|---:|
| Coarse | 1,125 | 11.90 | 0.24 |
| Fine | 1,419 | 12.71 | 0.19 |
| Refined | 1,501 | 12.88 | 0.18 |

### Coarse Mesh

The coarse mesh produced a maximum von Mises stress of 1,125 MPa, maximum displacement of 11.90 mm, and minimum factor of safety of 0.24.

These results exceeded the allowable stress and displacement limits.

**Stress Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/9835af3f-9238-4c29-9e85-0620805dd42f" />

**Displacement Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/15104637-72df-462c-846f-dcdf1103c81b" />

**Factor of Safety Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/9addfe34-4ea9-4164-addb-3269b50b5a84" />

### Fine Mesh

The fine mesh produced a maximum von Mises stress of 1,419 MPa, maximum displacement of 12.71 mm, and minimum factor of safety of 0.19.

The finer mesh captured higher stress concentrations and predicted slightly greater displacement.

**Stress Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/b6c35f98-a3c1-4779-b255-9b536e1a15e5" />

**Displacement Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/887c53ce-62e6-43e5-8925-5ee8b74cd6b4" />

**Factor of Safety Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/673ed9c9-5b0a-4fa4-b116-e82f540a4584" />

### Refined Mesh

The refined mesh produced a maximum von Mises stress of 1,501 MPa, maximum displacement of 12.88 mm, and minimum factor of safety of 0.18.

The results continued to show stresses above the material yield strength and displacement above the allowable limit.

**Stress Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/9d9a0a8b-7ac5-46cf-93ab-3083df5267f9" />

**Displacement Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/1e140a1d-ffd1-4857-85b2-4dfc277677d8" />

**Factor of Safety Plot**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/99bd0014-4cfc-4fbe-baff-882ce57097f2" />

### Mesh Comparison

As the mesh was refined, the maximum stress increased from 1,125 MPa to 1,501 MPa, while maximum displacement increased from 11.90 mm to 12.88 mm.

The displacement changed by approximately 1.3% between the fine and refined meshes, suggesting that displacement predictions were becoming more stable. However, the maximum stress continued to increase, so stress convergence was not demonstrated.

### Design Evaluation

| Requirement | Design 2 Result | Status |
|---|---|---|
| Maximum Stress | 1,501 MPa vs. 275 MPa yield | Fail |
| Maximum Displacement | 0.507 in vs. 0.005 in allowable | Fail |
| Minimum Factor of Safety | 0.18 vs. 4 required | Fail |

The linear elastic simulation predicts stresses significantly above yield strength. Therefore, the calculated deformation should not be interpreted as an accurate prediction of permanent physical deformation.

### Lessons Learned

Design 2 demonstrated that modifying the bracket geometry alone did not provide sufficient strength and stiffness to satisfy the design requirements. The highest stresses remained concentrated around the lower support and loading region.

Mesh refinement also demonstrated the importance of checking numerical convergence before relying on simulation results.

### Conclusion

Design 2 did not satisfy the required strength, stiffness, or factor of safety criteria under the applied 600 lbf load. Although the modified geometry changed the simulation results, additional design improvements are necessary.

The findings from Design 2 will be used to guide the development of Design 3, focusing on improving the vertical support and reducing stress concentrations.


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
