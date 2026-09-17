## Analyze


## Decide


## Communicate





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

$$
\sigma_{allow} = \frac{\sigma_y}{N}
$$

$$
\sigma_{allow} = \frac{60\text{ MPa}}{3}
$$

$$
\boxed{\sigma_{allow} = 20\text{ MPa}}
$$

These properties will be used for the stress and deflection calculations for both features of the motor mount.

## Feature 1

Feature 1 is the portion of the motor mount that attaches to the motor. For the analysis, this feature is approximated as a cantilever beam. The motor weight is neglected as specified in the assignment.

### Knowns and Unknowns

#### Knowns

- Applied force: $P = 300$ N
- Safety factor: $N = 3$
- Maximum allowable deflection: $\delta_{max} = 0.30$ mm
- Elastic modulus of PLA: $E = 3000$ MPa
- Yield strength of PLA: $\sigma_y = 60$ MPa
- Allowable stress: $\sigma_{allow} = 20$ MPa
- Motor diameter: approximately $28$ mm

#### Unknowns

The required cross-sectional geometry of Feature 1 must be determined using both strength and stiffness requirements.

The primary unknowns are:

- $b$ = width of the beam cross section
- $h$ = thickness of the beam cross section
- $I$ = area moment of inertia
- $\sigma_{max}$ = maximum bending stress
- Required cross-sectional dimensions based on yield strength
- Required cross-sectional dimensions based on the $0.30$ mm deflection limit

The larger cross-sectional requirement from the stress and deflection analyses will control the final design.
