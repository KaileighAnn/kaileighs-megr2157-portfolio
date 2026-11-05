# A08: Pulley System Design

## Objective

The objective of this assignment was to design a pulley system that transfers power between two parallel shafts while maintaining a minimum safety factor of 3. The design involved selecting a polyurethane belt, determining the minimum shaft diameter, evaluating journal bearings, and analyzing a supporting frame.

## Design Specifications

| Parameter | Value |
|---|---|
| Pulley Diameter | 3 in |
| Center Distance | 5 in |
| Rotational Speed | 1500 rpm |
| Initial Belt Tension | 5 lbf |
| Pulley Material | Aluminum 6061-T6 |
| Shaft Material | Hardened AISI 1060 Steel |
| Belt Material | Polyurethane |
| Belt Yield Strength | 471 psi |
| Minimum Safety Factor | 3 |

## Part 1: Belt Design

### Knowns and Unknowns

**Knowns:**

- Pulley radius: 1.5 in
- Initial tension: 5 lbf
- Yield strength: 471 psi
- Safety factor: 3
- Selected operating tensions: 7 lbf and 3 lbf

**Unknowns:**

- Transmitted torque
- Minimum belt area and diameter
- Belt circumference
- Required coefficient of friction

### Free-Body Diagram

<img width="520" height="247" alt="image" src="https://github.com/user-attachments/assets/e15cb2de-a4af-4a5b-ac67-e41d33c496f8" />

**Figure 1.** Belt and pulley free-body diagram.

### Equations and Calculations

<img width="765" height="895" alt="image" src="https://github.com/user-attachments/assets/e8b235f8-50d3-4bf4-9abd-5f90ca09840d" />


**Figure 2.** Handwritten belt design calculations showing belt tension, transmitted torque, allowable stress, minimum cross-sectional area, minimum belt diameter, belt length, and outer circumference.

### Belt Selection

A 1/4-inch polyurethane rubber belt was selected from McMaster-Carr (Part #3044K606). The calculated outer circumference was 20.210 inches, which falls within the available 12.25–24-inch range.

<img width="2172" height="724" alt="image" src="https://github.com/user-attachments/assets/48f490d6-cec2-4d9e-8c7c-34313243b51a" />

**Figure 3.** Polyurethane round belt selection from McMaster-Carr.

**Actual Belt Area:**

    A = π(0.25)² / 4

    A = 0.04909 in²

**Actual Safety Factor:**

    SF = 471 / (7 / 0.04909)

    SF = 3.30

The selected belt meets the minimum tensile safety factor of 3. No-slip operation requires an effective friction coefficient of at least 0.270, which must be verified for the selected belt and pulley.

---

## Part 2: Shaft Design

### Knowns and Unknowns

**Knowns:**

- Shaft material: Hardened AISI 1060 steel
- Assumed yield strength: 60,000 psi
- Torque: 6 in-lbf
- Transverse load: 10 lbf
- Assumed bearing spacing: 1 in
- Safety factor: 3

**Unknowns:**

- Maximum bending moment
- Minimum shaft diameter
- Actual shaft safety factor

### Free-Body Diagram

<img width="528" height="288" alt="image" src="https://github.com/user-attachments/assets/792e63d5-8bf1-4899-9bf9-2ea6e552c136" />

**Figure 4.** Shaft free-body diagram.

### Equations and Calculations

<img width="793" height="1012" alt="image" src="https://github.com/user-attachments/assets/93bf05f2-dd91-4f04-b44a-b9f3f7fe5848" />


**Figure 5.** Handwritten shaft design calculations showing bearing reactions, maximum bending moment, minimum and selected shaft diameters, bending stress, torsional shear stress, equivalent stress, and safety factor.

The selected 3/8-inch shaft satisfies the minimum static yielding safety factor under the assumed loading and material properties.

---

## Part 3: Journal Bearing Design

### Knowns and Unknowns

**Knowns:**

- Shaft diameter: 0.375 in
- Rotational speed: 1500 rpm
- Load per bearing: 5 lbf
- Bearing length: 0.5 in

**Unknowns:**

- Bearing pressure
- Surface velocity
- PV rating
- Suitable bearing material

### Free-Body Diagram

<img width="328" height="195" alt="image" src="https://github.com/user-attachments/assets/1fc80d63-e8cc-41de-add6-ecdcb51a6075" />

**Figure 6.** Journal bearing free-body diagram.

### Equations and Calculations

<img width="658" height="522" alt="image" src="https://github.com/user-attachments/assets/5165f9c9-251b-4fca-823f-8a4109625e6b" />

**Figure 7.** Handwritten journal bearing calculations showing projected area, bearing pressure, surface velocity, and PV rating.

### Material Selection

Porous bronze (SAE 841) was selected as the journal bearing material using Table 4 on page 2440 of the Machinery's Handbook.

| Parameter | Calculated | Maximum Allowable |
|---|---|---|
| Bearing Pressure | 26.67 psi | 4500 psi |
| Surface Velocity | 147.26 ft/min | 1500 ft/min |
| PV Rating | 3927 | 50,000 |

The calculated pressure, surface velocity, and PV rating are all below the maximum allowable limits for porous bronze. Therefore, the selected bearing meets the listed mechanical operating limits. Operating temperature must also remain below 160°F.

---

## Part 4: Frame Design

A 6061-T6 aluminum frame was selected to support the two pulleys and maintain a center distance of 5 inches.

### Proposed Dimensions

| Parameter | Value |
|---|---|
| Base Plate | 8 × 4 × 0.25 in |
| Center Distance | 5 in |
| Support Thickness | 0.25 in |
| Support Width | 1 in |
| Frame Material | Aluminum 6061-T6 |

### Frame Analysis

A simplified support member was modeled as a simply supported beam with a 10 lbf center load over a 5-inch span.

**Maximum Bending Moment:**

$$
M=\frac{FL}{4}=\frac{10(5)}{4}
=12.5\text{ in-lbf}
$$

**Moment of Inertia:**

$$
I=\frac{bh^3}{12}
$$

$$
I=\frac{1(0.25)^3}{12}
=0.001302\text{ in}^4
$$

**Maximum Bending Stress:**

$$
\sigma=\frac{Mc}{I}
$$

$$
\sigma=\frac{12.5(0.125)}{0.001302}
=1200\text{ psi}
$$

**Safety Factor:**

Using an assumed aluminum yield strength of 35,000 psi:

$$
SF=\frac{35000}{1200}=29.17
$$

**Maximum Deflection:**

$$
\delta=\frac{FL^3}{48EI}
$$

$$
\delta=
\frac{10(5)^3}
{48(10\times10^6)(0.001302)}
$$

$$
\boxed{\delta=0.0020\text{ in}}
$$

The simplified frame member satisfies the minimum safety factor requirement. The complete frame, including its bearing mounts and connections, would require additional verification.

**Figure 4.** Proposed pulley support frame.

*Insert a labeled sketch of the frame showing the base, supports, shafts, and 5-inch center distance.*

---

## Part 5: Engineering Lessons Learned

This assignment helped me understand how belt tension, torque, shaft loading, and bearing selection are connected. I learned that the difference between the tight-side and loose-side belt tensions determines the torque transmitted, while the combined belt forces create loads that must be supported by the shafts and bearings.

I also learned how to calculate the minimum shaft diameter using bending and torsional stresses and how bearing pressure and surface velocity are used to evaluate journal bearing materials. This project showed me how individual calculations work together when designing a complete mechanical system.

---

## Project Completion Time

| Task | Time |
|---|---|
| Research and Design Selection | To be recorded |
| Belt Calculations | To be recorded |
| Shaft Calculations | To be recorded |
| Bearing Calculations | To be recorded |
| Frame Analysis | To be recorded |
| Documentation | To be recorded |
| **Total** | **To be recorded** |

## References

1. [McMaster-Carr — Polyurethane Round Belts](https://www.mcmaster.com/products/round-belts/round-belts-8/)
2. *Machinery's Handbook*, Simple Stresses, p. 217.
3. *Machinery's Handbook*, Journal Bearings, Table 4, p. 2440.
4. D. J. Dunn, *Solid Mechanics — Dynamics: Tutorial — Pulley Drive Systems*.
5. Wang et al., *Strain-induced Structural and Dynamic Changes in Segmented Polyurethane Elastomers*.
