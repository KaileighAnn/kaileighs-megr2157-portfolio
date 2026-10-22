# A07 – Bracket FEA

## Objective

The objective of this assignment is to use Finite Element Analysis (FEA) to evaluate and improve the bracket designed in A05 and modeled in A06. The bracket will be analyzed for stress, displacement, safety factor, and mass. Geometry changes will be made to improve strength, stiffness, and weight.

## Original Bracket Design

The original bracket was designed using strength and stiffness calculations in A05 and modeled parametrically in SolidWorks for A06. This model will serve as the starting point for the FEA simulations.

### Design Requirements

| Parameter | Value |
|---|---|
| Material | Aluminum 6061-T6 |
| Applied Load | 600 lbf downward |
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

A linear static FEA was performed in SolidWorks Simulation to evaluate the original bracket under a 600 lbf downward load. Three mesh densities were compared to evaluate convergence within 7%.

### Simulation Setup

- **Study Type:** Static
- **Material:** Aluminum 6061-T6
- **Fixtures:** Two interior mounting faces fixed
- **Applied Force:** 600 lbf downward on the cylindrical feature
- **Mesh Quality:** High
- **Mesh Sizes:** Coarse, Fine, Refined
- **Failure Criterion:** Maximum von Mises Stress

### Mesh Convergence

| Mesh Size | Max Stress (psi) | Max Displacement (in) | Minimum Safety Factor |
|---|---|---|---|
| Coarse | 164,600 | 0.426 | 0.24 |
| Fine | 220,500 | 0.601 | 0.18 |
| Refined | 240,900 | 0.618 | 0.17 |

The fine and refined mesh results differed by 8.47% in maximum stress and 2.75% in maximum displacement. Displacement met the 7% convergence requirement, but stress did not.

Additional mesh refinement is needed to verify stress convergence.

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

## Design 2 – Modified Bracket

### Design

Design 2 was developed as an improvement to Design 1 to increase the strength and stiffness of the bracket. The geometry was modified while maintaining a symmetrical design and the original mounting and loading features.

The updated model was created in SOLIDWORKS using Aluminum 6061-T6.

### Design Modifications

Design 2 was modified to improve the bracket's strength and stiffness while maintaining the original mounting and loading conditions.

The updated geometry includes:

- Overall upper bracket width of 3.10 in.
- Upper section height of 1.34 in.
- Center vertical support width of 1.34 in.
- Lower cylindrical feature diameter of 1.10 in.
- Symmetrical geometry about the vertical centerline.
- Retained upper mounting opening and lower loading feature.

The modified bracket was evaluated using coarse, fine, and refined meshes to compare its structural performance with Design 1.

### Modified CAD Model

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/1c33c237-41e4-40b0-a1b3-a0abf05ca6a6" />

*Figure. Dimensioned sketch of the modified bracket geometry for Design 2.*

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

The fine and refined mesh results were compared to determine whether Design 2 satisfied the 7% convergence requirement.

**Percentage Difference Formula:**

Percentage Difference = |Refined − Fine| / Refined × 100

**Stress Convergence**

Percentage Difference = |1,501 − 1,419| / 1,501 × 100

**Stress Difference = 5.46%**

**Displacement Convergence**

Percentage Difference = |12.88 − 12.71| / 12.88 × 100

**Displacement Difference = 1.32%**

| Measurement | Percentage Difference | Requirement | Result |
|---|---|---|---|
| Maximum Stress | 5.46% | Less than 7% | Met |
| Maximum Displacement | 1.32% | Less than 7% | Met |

Both measurements satisfied the 7% convergence criterion between the fine and refined meshes. However, the maximum stress continued to increase with refinement, so further verification may be useful.

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

#### Design

Design 3 was developed to improve the strength and stiffness of the bracket after evaluating the results from Designs 1 and 2.

The main modification was increasing the thickness of the middle support section to reduce bending and displacement under the applied load.

#### Design Modifications

The following changes were made in SOLIDWORKS:

- Reduced the cut-extrude depth from 0.90 in to 0.60 in to increase the thickness of the middle support.
- Maintained the overall upper mounting geometry.
- Retained the lower cylindrical loading feature.
- Continued using Aluminum 6061-T6.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/240af944-9dd3-45ce-9009-2d754a036c01" />

The updated geometry was evaluated using coarse, fine, and refined meshes.

#### Finite Element Analysis (FEA)

Three linear static simulations were completed in SOLIDWORKS Simulation to evaluate the modified bracket.

##### Simulation Settings

| Parameter | Value |
|---|---|
| Study Type | Linear Static |
| Material | Aluminum 6061-T6 |
| Applied Load | 600 lbf downward |
| Fixtures | Two upper interior mounting faces |
| Load Location | Lower cylindrical feature |
| Mesh Quality | High |
| Failure Criterion | Maximum von Mises Stress |
| Yield Strength | 40,000 psi |
| Required Factor of Safety | 4.0 |
| Maximum Allowable Displacement | 0.005 in |

#### Mesh Generation

Three mesh densities were used to evaluate how element size affected the simulation results.

| Mesh | Maximum Element Size | Minimum Element Size | Total Nodes | Total Elements |
|---|---|---|---|---|
| Coarse | 0.30 in | 0.15 in | 2,980 | 1,660 |
| Fine | 0.15 in | 0.075 in | To be recorded | To be recorded |
| Refined | 0.10 in | 0.05 in | To be recorded | To be recorded |

#### FEA Results

| Mesh | Maximum Stress (MPa) | Maximum Displacement (mm) | Minimum Safety Factor |
|---|---|---|---|
| Coarse | 122.8 | 0.4057 | 2.24 |
| Fine | 149.7 | 0.4202 | 1.84 |
| Refined | 178.6 | 0.4245 | 1.54 |

#### Coarse Mesh Analysis

The coarse mesh was used for the initial simulation of Design 3.

##### Von Mises Stress

The maximum von Mises stress was approximately 122.8 MPa.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/124d1957-9af5-40d7-a61a-82ea536f75a9" />

*Figure. Von Mises stress distribution for the coarse mesh.*

##### Displacement

The maximum resultant displacement was 0.4057 mm (0.01597 in), exceeding the allowable displacement of 0.005 in.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/3d374132-8255-4c01-a357-df5d93affe5e" />

*Figure. Resultant displacement distribution for the coarse mesh.*

##### Factor of Safety

The minimum factor of safety was approximately 2.24, below the required value of 4.0.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/a018409e-04db-4099-ae57-261383cee623" />

*Figure. Factor of safety distribution for the coarse mesh.*

#### Fine Mesh Analysis

A finer mesh was generated to improve the resolution of the stress and displacement results.

##### Von Mises Stress

The maximum von Mises stress increased to approximately 149.7 MPa.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/38b2f7e0-d418-4de7-ac1f-9a6f3de0a65b" />

*Figure. Von Mises stress distribution for the fine mesh.*

##### Displacement

The maximum resultant displacement increased to 0.4202 mm (0.01654 in).

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/8e58c20c-70ce-4fdc-8ca1-add55bf3c974" />

*Figure. Resultant displacement distribution for the fine mesh.*

##### Factor of Safety

The minimum factor of safety decreased to approximately 1.84.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/27e11f40-da3f-4a96-b5d5-8b4824109b4a" />

*Figure. Factor of safety distribution for the fine mesh.*

#### Refined Mesh Analysis

A refined mesh was generated for the final evaluation of Design 3.

##### Von Mises Stress

The maximum von Mises stress increased to approximately 178.6 MPa.

Although this value remained below the material yield strength of approximately 275 MPa, it exceeded the allowable stress of 68.75 MPa required for a safety factor of 4.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/4bc874d4-42f3-42ef-9268-87efd9c723bf" />

*Figure. Von Mises stress distribution for the refined mesh.*

##### Displacement

The maximum resultant displacement was approximately 0.4245 mm (0.01671 in).

This exceeded the maximum allowable displacement of 0.005 in.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/732b50b4-087b-46ce-bdc0-934ce5f44e23" />

*Figure. Resultant displacement distribution for the refined mesh.*

##### Factor of Safety

The minimum factor of safety was approximately 1.54, which was below the required value of 4.0.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/ddc663e3-cce2-4814-8a6a-9a8c8b89155e" />

*Figure. Factor of safety distribution for the refined mesh.*

#### Mesh Convergence Evaluation

The fine and refined mesh results were compared to determine whether the simulation satisfied the 7% convergence requirement.

**Percentage Difference Formula:**

Percentage Difference = |Refined − Fine| / Refined × 100

**Stress Convergence**

Percentage Difference = |178.6 − 149.7| / 178.6 × 100

**Stress Difference = 16.18%**

**Displacement Convergence**

Percentage Difference = |0.4245 − 0.4202| / 0.4245 × 100

**Displacement Difference = 1.01%**

| Measurement | Percentage Difference | Requirement | Result |
|---|---|---|---|
| Maximum Stress | 16.18% | Less than 7% | Not Met |
| Maximum Displacement | 1.01% | Less than 7% | Met |

The displacement results satisfied the convergence requirement, but the stress results did not.

Additional mesh refinement would be necessary to verify stress convergence.

#### Final Design III Results

| Measurement | Design III Result | Requirement | Status |
|---|---|---|---|
| Maximum von Mises Stress | 178.6 MPa | 68.75 MPa allowable | Not Met |
| Maximum Displacement | 0.01671 in | 0.005 in maximum | Not Met |
| Minimum Factor of Safety | 1.54 | 4.0 minimum | Not Met |
| Material | Aluminum 6061-T6 | Aluminum 6061-T6 | Met |
| Applied Load | 600 lbf | 600 lbf | Met |
| Stress Mesh Convergence | 16.18% | Less than 7% | Not Met |
| Displacement Mesh Convergence | 1.01% | Less than 7% | Met |

#### Design III Analysis

The FEA results showed that increasing the thickness of the middle support substantially improved the bracket's strength and stiffness compared with Designs 1 and 2.

The maximum stress and displacement decreased significantly, while the minimum factor of safety increased.

However, the refined mesh results still exceeded the allowable stress and displacement limits.

The stress results also continued to increase with mesh refinement, indicating that further refinement was needed to establish convergence.

#### Lessons Learned

Design 3 demonstrated the importance of the middle support thickness in resisting bending under the applied load.

Increasing the amount of material in this region reduced displacement and stress compared with the previous designs.

The mesh refinement study also showed that the coarse mesh predicted a higher factor of safety than the refined mesh, demonstrating why mesh convergence must be evaluated.

#### Design III Conclusion

Design 3 showed substantial improvements over Designs 1 and 2. However, the final design did not satisfy the required factor of safety of 4.0 or maximum displacement of 0.005 in.

The results demonstrated that increasing the thickness of the middle support improved structural performance, but additional modifications would be required to satisfy all design requirements.

## Final Results

| Measurement | Design I | Design II | Design III |
|---|---|---|---|
| Maximum Stress | 240,900 psi | 217,700 psi | 25,904 psi |
| Maximum Deflection | 0.618 in | 0.507 in | 0.01671 in |
| Mass | 0.38 lb | 0.38 lb | 0.44 lb |
| Minimum Safety Factor | 0.17 | 0.18 | 1.54 |
| Number of Elements | 30,268 | 49,865 | 34,967 |


### Design Comparison

Designs 1, 2, and 3 were compared using the refined mesh results to evaluate improvements in strength, stiffness, and factor of safety.

- **Maximum Stress:** Decreased from 240,900 psi in Design 1 to 217,700 psi in Design 2 and 25,904 psi in Design 3.
- **Maximum Displacement:** Decreased from 0.618 in in Design 1 to 0.507 in in Design 2 and 0.01671 in in Design 3.
- **Minimum Factor of Safety:** Increased from 0.17 in Design 1 to 0.18 in Design 2 and 1.54 in Design 3.
- **Mass:** Increased from 0.38 lb in Designs 1 and 2 to 0.44 lb in Design 3.

Design 3 provided the greatest improvement in strength and stiffness. However, none of the three designs met the required factor of safety of 4.0 or maximum displacement of 0.005 in.

Further modifications would be necessary to satisfy all design requirements.


## Lessons Learned

This assignment demonstrated how FEA can be used to identify weak areas in a design and evaluate improvements.

- Increasing the thickness of the middle support significantly reduced stress and displacement.
- Finer meshes provided more detailed results and helped identify stress concentrations.
- Design 3 performed the best but required additional material, increasing its mass.
- Mesh convergence is important because results can change as the mesh becomes finer.
- Although Design 3 improved significantly, it still did not meet the required factor of safety or displacement limit.

Overall, I learned how to use SOLIDWORKS Simulation to compare different designs and make improvements based on FEA results.


## Time Spent

| Activity | Time |
|---|---|
| FEA Setup | 1.0 hr |
| Mesh Validation | 1.5 hrs |
| Design Optimization | 2.0 hrs |
| Documentation | 1.0 hr |
| **Total** | **5.5 hrs** |


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

A linear static FEA was performed in SOLIDWORKS Simulation using Aluminum 6061-T6.

The upper hole was fixed, and a 600 lbf downward load was applied to the lower hole.

| Measurement | Simulation Result |
|---|---|
| Maximum von Mises Stress | 0.02674 MPa |
| Maximum Displacement | 0.0004129 mm |
| Minimum Factor of Safety | Approximately 10,280 |

The simulation showed the highest stress around the lower hole and the greatest displacement near the bottom of the link.

These are the initial simulation results. Further validation would be needed before drawing conclusions about the link's structural performance.


#### Von Mises Stress

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/9b62d90d-02c1-4cd4-8acc-02ebd9673dfd" />

*Figure. Von Mises stress distribution of the link.*

#### Displacement

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/ccfa43f6-c101-4854-bbc3-071dfdb698f7" />

*Figure. Resultant displacement of the link.*

#### Factor of Safety

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/44674ba0-a9e1-4282-9d92-e5a15d79fbe4" />

*Figure. Factor of safety distribution of the link.*


### Link FEA Conclusion

The link was analyzed using SOLIDWORKS Simulation with a 600 lbf downward load. The initial results showed low stress and displacement values and a high factor of safety.

However, the unusually low results require further validation before confirming that the link meets the design requirements.

This analysis provided additional experience with applying fixtures, loads, and interpreting FEA results.


## CAD Files

The following SolidWorks CAD files were used to complete the bracket and link finite element analyses.

- [Download Design 1 CAD Model](CAD/Design1.SLDPRT)
- [Download Design 2 CAD Model](CAD/Design2.SLDPRT)
- [Download Design 3 CAD Model](CAD/Design3.SLDPRT)
- [Download Link CAD Model](CAD/A07_Link.SLDPRT)


