# A5 – Bracket Design

## Objective

The objective of this assignment is to design a bracket that can safely support a horizontal load between 500 and 800 lbf. The bracket will be analyzed using stress and stiffness equations to determine the required dimensions of each feature.

Each feature will be analyzed using free body diagrams, strength calculations, and deflection calculations. A safety factor of 4 and a maximum deflection of 0.005 in will be used. The final dimensions will be determined by comparing the stress and stiffness requirements.

## Analyze

The bracket was separated into five features labeled A through E. Each feature was analyzed individually, with forces and dimensions from earlier features being carried into later calculations.

### Design Requirements

- Applied Load: **600 lbf**
- Safety Factor: **4**
- Maximum Deflection: **0.005 in**
- Material: **Aluminum 6061-T6**
- Yield Strength: **40,000 psi**
- Modulus of Elasticity: **10 × 10<sup>6</sup> psi**
- Direct shear failure was neglected.
- Shear deflection was neglected.

Since the strap has two loaded ends, the total load on the bracket is:

**F<sub>strap</sub> = 2F = 2(600) = 1200 lbf**

Using a safety factor of 4:

**σ<sub>allow</sub> = S<sub>y</sub> / SF = 40,000 / 4 = 10,000 psi**

## Stress Analysis

Each of the five bracket features was analyzed using the appropriate stress equations. For each feature, I identified the knowns, unknowns, assumptions, created a free body diagram, developed the algebraic model, and calculated the required dimension.

### Feature A

Feature A supports the polyester strap and is analyzed first because its resulting dimension is used in the following feature calculations.

<img width="850" height="788" alt="image" src="https://github.com/user-attachments/assets/10e970db-5f11-4de4-9114-c0cf800c5590" />

### Feature B

Feature B connects Feature A to the upper portion of the bracket. The load from Feature A is transferred into Feature B, which is modeled as an axially loaded bar.

<img width="871" height="756" alt="image" src="https://github.com/user-attachments/assets/cee9e0b0-742a-4db4-9c59-940b06b215ee" />

### Feature C

Feature C transfers the load through the T-beam and is modeled as a simply supported beam with a concentrated load at the center.

<img width="1313" height="1198" alt="image" src="https://github.com/user-attachments/assets/58b5b483-11ed-4ff1-9177-d348a2784008" />

### Feature D

Feature D transfers the load from Feature C into the upper portion of the T-beam. The minimum thickness was determined using the load carried from the previous feature.

<img width="1363" height="1154" alt="image" src="https://github.com/user-attachments/assets/d23e08d1-1f87-4a0c-8983-50a94880c91b" />

### Feature E

Feature E consists of two symmetric sections that transfer the load into the rigid T-beam. Each section carries half of the total load and is analyzed using bending stress.

<img width="1334" height="1179" alt="image" src="https://github.com/user-attachments/assets/9b7294cf-3e2e-46db-a058-ff0e9711b379" />

## Stiffness Analysis

Each feature was then analyzed using a maximum allowable deflection of **0.005 in**.

### Feature A

<img width="1303" height="1207" alt="image" src="https://github.com/user-attachments/assets/e87b52f7-955f-40b4-88f5-7179f0c8ecc3" />

### Feature B

<img width="1347" height="1167" alt="image" src="https://github.com/user-attachments/assets/d3110a26-9c46-4d49-97c2-b7b4149ac518" />

### Feature C

<img width="1254" height="1254" alt="image" src="https://github.com/user-attachments/assets/938b4e42-ee99-4a28-9cc4-b39d5992455d" />

### Feature D

<img width="1303" height="1207" alt="image" src="https://github.com/user-attachments/assets/b35d88d8-82e6-442b-940d-77094d54621f" />

### Feature E

<img width="1303" height="1207" alt="image" src="https://github.com/user-attachments/assets/43465e33-3c8e-4729-b371-4954e4ad1d78" />

## Multiview Sketches

Two multiview sketches were created using the dimensions determined from the stress and stiffness analyses.

### Stress Analysis Design

<img width="694" height="610" alt="image" src="https://github.com/user-attachments/assets/4a34cb19-5d8b-4575-9a50-b8350e57d25b" />

### Stiffness Analysis Design

<img width="1334" height="1179" alt="image" src="https://github.com/user-attachments/assets/33730d7d-6dcc-4edd-bd39-c0fdf6945c00" />

## Lessons Learned

### Governing Failure Mode

Stress governed the design for all five features because the stress calculations required larger dimensions than the stiffness calculations.

### Error Propagation

The dimensions of earlier features were used in later calculations, so an error in one calculation could affect the dimensions of the following features.

### Assumption Sensitivity

The calculations assume symmetric loading, small deflections, elastic material behavior, and neglected shear deformation and stress concentrations. Changing these assumptions could change the required dimensions.

## Time

- Research and setup: **1 hour**
- Stress analysis: **3 hours**
- Stiffness analysis: **2.5 hours**
- Multiview sketches: **1 hour**
- Portfolio documentation: **1.5 hours**

**Total Time: 9 hours**
