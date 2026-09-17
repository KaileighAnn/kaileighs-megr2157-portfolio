## Analyze


## Decide


## Communicate


# A04 - Motor Mount

## Analyze

### Objective

The goal of this assignment is to design a motor mount for a 24V DC gear motor. The mount must support an applied load of 300 N while meeting both strength and stiffness requirements.

The design will be analyzed using beam bending equations with a safety factor of 3 and a maximum allowable deflection of 0.30 mm.

The mount is divided into two main features:

- **Feature 1:** Attaches to the motor
- **Feature 2:** Attaches to the rigid wall

Each feature will be analyzed separately before creating the final motor mount.

### Motor

The motor used for this design is the **Brushed 24V DC Gear Motor with a 99.5:1 Planetary Gearbox**.

Important dimensions from the motor drawing will be used to determine the size and location of the shaft and mounting holes in the final design.

### Material Selection

I chose **PLA** for the motor mount because its stiffness makes it a good option for limiting deflection.

Material properties used:

| Property | Value |
|---|---:|
| Material | PLA |
| Elastic Modulus, $E$ | 3000 MPa |
| Yield Strength, $\sigma_y$ | 60 MPa |
| Safety Factor, $N$ | 3 |
| Maximum Deflection | 0.30 mm |

The allowable stress is:

$$
\sigma_{allow}=\frac{\sigma_y}{N}
$$

$$
\sigma_{allow}=\frac{60}{3}=20\text{ MPa}
$$

$$
\boxed{\sigma_{allow}=20\text{ MPa}}
$$

---

## Feature 1

Feature 1 is the portion of the mount that attaches to the motor. For the beam calculations, I simplified this feature as a cantilever beam.

### Knowns and Unknowns

**Knowns:**

- $P=300$ N
- $N=3$
- $\delta_{max}=0.30$ mm
- $E=3000$ MPa
- $\sigma_y=60$ MPa
- $\sigma_{allow}=20$ MPa

**Unknowns:**

- Required cross-sectional geometry
- Required dimension based on strength
- Required dimension based on deflection

### Free Body Diagram

[INSERT FEATURE 1 FBD HERE]

The 300 N load is applied at the free end of the feature. The opposite end is treated as fixed for the beam analysis.
