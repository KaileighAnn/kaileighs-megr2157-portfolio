# A5 – Bracket Design

## Objective

The objective of this assignment is to design a bracket that can safely support a horizontal load between 500 and 800 lbf. The bracket will be analyzed using stress and stiffness equations to determine the required dimensions of each feature.

Each feature will be analyzed using free body diagrams, strength calculations, and deflection calculations. A safety factor of 4 and a maximum deflection of 0.005 in will be used. The final dimensions will be determined by comparing the stress and stiffness requirements.

## Design Requirements

The bracket will be designed using the following requirements:

- Applied load: **F = 600 lbf**
- Safety Factor: **SF = 4**
- Maximum allowable deflection: **0.005 in**
- Material: **Aluminum 6061-T6**
- Yield Strength: **S<sub>y</sub> = 40,000 psi**
- Modulus of Elasticity: **E = 10 × 10<sup>6</sup> psi**
- Direct shear failure is neglected.
- Shear deflection is neglected.
- The bracket is assumed to be symmetric.

### T-Beam Dimensions

From the provided rigid T-beam:

- **a = 0.498 in**
- **b = 0.9992 in**
- **c = 1.499 in**

### Allowable Stress

The allowable stress was determined using the yield strength and safety factor:

**σ<sub>allow</sub> = S<sub>y</sub> / SF**

σ<sub>allow</sub> = 40,000 / 4

**σ<sub>allow</sub> = 10,000 psi**

# Stress Analysis

## Feature A – Cylindrical Strap Support

Feature A supports the polyester strap. Since the bracket is symmetric, the total applied load is divided equally between the two sides. Feature A is modeled as a cantilever beam.

### Known Values

- Applied Load: **F = 600 lbf**
- Load per side: **P = 300 lbf**
- Safety Factor: **SF = 4**
- Material: **Aluminum 6061-T6**
- Yield Strength: **40,000 psi**
- Allowable Stress: **10,000 psi**

### Unknown

- Minimum required diameter of Feature A, **d<sub>A</sub>**

### Assumptions

1. Feature A is modeled as a cantilever beam.
2. The load is divided equally due to symmetry.
3. Direct shear failure is neglected.
4. Stress concentrations are neglected.
5. The material remains elastic.
6. Feature A has a circular cross section.

### FBD and Calculations

The FBD, algebraic model, and numerical calculations for Feature A are shown below.

**[Insert handwritten calculations here]**
