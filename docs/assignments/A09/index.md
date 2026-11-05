
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

**Figure 1.** Belt and pulley free-body diagram.

*Insert FBD showing the tight-side tension (7 lbf), loose-side tension (3 lbf), pulley radius (1.5 in), and shaft reaction.*


### Equations and Calculations

**Belt Tensions:**

T₀ = (T₁ + T₂) / 2

T₀ = (7 + 3) / 2 = 5 lbf

**Transmitted Torque:**

M = (T₁ − T₂) × r

M = (7 − 3) × 1.5

**M = 6 in·lbf**

**Allowable Belt Stress:**

σ_allow = Sᵧ / SF

σ_allow = 471 / 3

**σ_allow = 157 psi**

**Minimum Cross-Sectional Area:**

A_min = T₁ / σ_allow

A_min = 7 / 157

**A_min = 0.04459 in²**

**Minimum Belt Diameter:**

d_min = √(4A / π)

d_min = √(4 × 0.04459 / π)

**d_min = 0.2383 in**

**Belt Length:**

L = 2C + πD

L = 2(5) + π(3)

**L = 19.425 in**

**Outer Circumference:**

L_outer = L + πd

L_outer = 19.425 + π(0.25)

**L_outer = 20.210 in**

### Belt Selection

A 1/4-inch polyurethane rubber belt was selected from McMaster-Carr (Part #3044K606). The calculated outer circumference was 20.210 inches, which falls within the available 12.25–24-inch range.

<img width="2172" height="724" alt="image" src="https://github.com/user-attachments/assets/48f490d6-cec2-4d9e-8c7c-34313243b51a" />

**Figure 2.** Polyurethane round belt selection from McMaster-Carr.

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

**Figure 2.** Shaft free-body diagram.

*Insert a simply supported shaft with a 10 lbf center load, two bearing reactions of 5 lbf, and a 1-inch bearing spacing.*

### Equations and Calculations

**Bearing Reactions:**

$$
R_A=R_B=\frac{10}{2}=5\text{ lbf}
$$

**Maximum Bending Moment:**

$$
M=\frac{FL}{4}
$$

$$
M=\frac{10(1)}{4}=2.5\text{ in-lbf}
$$

**Minimum Shaft Diameter:**

Using combined bending and torsion:

$$
d_{\min}=
\left[
\frac{16(SF)\sqrt{4M^2+3T^2}}
{\pi S_y}
\right]^{1/3}
$$

$$
d_{\min}=
\left[
\frac{16(3)\sqrt{4(2.5)^2+3(6)^2}}
{\pi(60000)}
\right]^{1/3}
$$

$$
\boxed{d_{\min}=0.1432\text{ in}}
$$

**Selected Shaft Diameter:**

$$
d=0.375\text{ in}
$$

**Bending Stress:**

$$
\sigma_b=\frac{32M}{\pi d^3}=482.89\text{ psi}
$$

**Torsional Shear Stress:**

$$
\tau=\frac{16T}{\pi d^3}=579.47\text{ psi}
$$

**Equivalent Stress:**

$$
\sigma_{VM}=\sqrt{\sigma_b^2+3\tau^2}
$$

$$
\sigma_{VM}=1113.79\text{ psi}
$$

**Safety Factor:**

$$
SF=\frac{60000}{1113.79}=53.87
$$

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

**Figure 3.** Journal bearing free-body diagram.

*Insert the shaft supported by two journal bearings, each carrying a 5 lbf reaction.*

### Equations and Calculations

**Projected Bearing Area:**

$$
A=dL
$$

$$
A=(0.375)(0.5)=0.1875\text{ in}^2
$$

**Bearing Pressure:**

$$
P=\frac{W}{dL}
$$

$$
P=\frac{5}{0.1875}=26.67\text{ psi}
$$

**Surface Velocity:**

$$
V=\frac{\pi dN}{12}
$$

$$
V=\frac{\pi(0.375)(1500)}{12}
=147.26\text{ ft/min}
$$

**PV Rating:**

$$
PV=P(V)
$$

$$
PV=(26.67)(147.26)
$$

$$
\boxed{PV=3927\text{ psi-ft/min}}
$$

### Material Selection

Oil-impregnated sintered bronze (SAE 841) was selected as the preliminary journal bearing material.

| Parameter | Calculated | Reference Limit |
|---|---|---|
| Pressure | 26.67 psi | 2000 psi |
| Velocity | 147.26 ft/min | 1200 ft/min |
| PV | 3927 | 50,000 |

The calculated operating conditions are below the referenced limits for porous bronze bearings. The final selection should be checked against Table 4 on page 2440 of the assigned *Machinery's Handbook* edition.

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
