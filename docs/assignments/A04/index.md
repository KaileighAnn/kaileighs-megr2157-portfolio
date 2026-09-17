# A04 - Motor Mount

## Objective

The objective of this assignment is to design a motor mount for a 24V DC gear motor subjected to a 300 N load. The mount will be designed using beam bending equations and evaluated based on both yield strength and maximum deflection. A safety factor of 3 and a maximum allowable deflection of 0.30 mm will be used.

The motor mount will consist of two main features: one attached to the motor and one attached to a rigid wall. Both features will be analyzed separately to determine the required cross-sectional geometry. The final design will then be modeled parametrically in CAD with appropriate clearance holes and features to minimize deflection.

## Material Selection

For this motor mount, I selected **PLA (Polylactic Acid)** as the material. PLA was chosen because it has a relatively high stiffness compared to other common 3D printing materials, making it a good choice for limiting deflection in the motor mount.

The material properties used for the calculations are:

- **Material:** PLA
- **Elastic Modulus, E:** 3000 MPa
- **Yield Strength, σy:** 60 MPa
- **Safety Factor, N:** 3

The allowable stress is calculated using:

**σallow = σy / N**

**σallow = 60 MPa / 3**

**σallow = 20 MPa**

These properties will be used for the stress and deflection calculations for both features of the motor mount.

## Feature 1

Feature 1 is the portion of the motor mount that attaches to the motor. For the analysis, this feature is approximated as a cantilever beam. The motor weight is neglected as specified in the assignment.

### Knowns and Unknowns

#### Knowns

- Applied force: **P = 300 N**
- Safety factor: **N = 3**
- Maximum allowable deflection: **δmax = 0.30 mm**
- Material: **PLA**
- Elastic modulus: **E = 3000 MPa**
- Yield strength: **σy = 60 MPa**
- Allowable stress: **σallow = 20 MPa**
- Motor diameter: **28 mm**
- Base: **b = 30 mm**
- Width: **w = 30 mm**
- Motor weight is neglected
- Feature 1 is modeled as a cantilever beam

#### Unknowns

The following values will be determined using the beam bending equations:

- **h** = required height of Feature 1
- **Lstrength** = maximum allowable length based on yield strength
- **Ldeflection** = maximum allowable length based on the 0.30 mm deflection requirement
- **I** = area moment of inertia
- **Mmax** = maximum bending moment
- **σmax** = maximum bending stress
- **Lfinal** = final length selected for Feature 1

The results from the strength and deflection calculations will be compared, and the more restrictive value will be used to determine the final geometry of Feature 1.

### Free Body Diagram

The free body diagram below shows Feature 1 modeled as a cantilever beam. The 300 N load is applied downward at the free end of the beam, while the opposite end is fixed.

The cross section is modeled as a rectangle with a width **b** and height **h**.

<img width="682" height="495" alt="image" src="https://github.com/user-attachments/assets/2a7f9c33-ad4f-442c-bdd0-09c5b2c0623d" />

