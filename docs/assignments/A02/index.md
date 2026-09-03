# A2 – Truss Stress Analysis

## Objective

The objective of this project was to design and analyze a truss that can support the given loads while keeping the design strong, stable, and lightweight.

## Analyze
# Assignment 2: Truss Stress

## Introduction and Design Requirements

For this assignment, I designed a lightweight planar truss that can support two applied loads while staying within the required dimensions. I used statics to determine the forces in each truss member and then used stress and material strength to determine the required cross-sectional area of the members and connecting pins. After completing the hand calculations, I created the truss in CAD and compared the CAD weight to my calculated weight.

<img width="317" height="215" alt="image" src="https://github.com/user-attachments/assets/9153125e-1b39-4e37-a614-262ddf469ea3" />


### Given

- a = 0.4 m
- b = 0.3 m
- P = 20–30 kN
- Selected load: P = 24 kN
- Truss safety factor = 3.5
- Pin safety factor = 4
- Pin shear yield strength = 170 ksi
- Pin density = 0.278 lb/in³
- Truss material = A500 structural steel
- A = pin support
- B = roller support
- Pin connection = single shear

---

# Step 1: Truss Geometry and Statics

## Initial Truss Design

This was my original truss design. I wanted to keep the design simple and lightweight, so I initially created the truss with only eight members. After looking back at what I learned in Statics, I realized that I needed to check whether the truss had enough members to be statically determinate and stable.

<img width="555" height="322" alt="image" src="https://github.com/user-attachments/assets/27c03a90-ec04-422c-bc32-567ee54f0e0d" />


<p align="center">
m + r = 2j<br>
8 + 3 = 2(6)<br>
11 ≠ 12
</p>

From this check, I realized my original design needed another member. I also noticed that the middle section formed a rectangle instead of being completely triangularized. To fix this, I added the diagonal member ED, which divided the middle section into triangles and gave the truss nine total members.

<img width="555" height="256" alt="image" src="https://github.com/user-attachments/assets/3a4e86bb-bbd4-4c49-bbba-b6f109dfd8aa" />


<p align="center">
m + r = 2j<br>
9 + 3 = 2(6)<br>
12 = 12
</p>

After adding the diagonal member, the truss satisfied the relationship `m + r = 2j`. This gave me the correct number of members and reactions for a statically determinate planar truss, and the added diagonal also helped triangularize the structure. I decided to continue with this geometry for the remainder of the assignment.

---

## Truss Dimensions

After deciding on my final truss design, I calculated the length of each member using the given dimensions of `a = 0.4 m` and `b = 0.3 m`. The horizontal and vertical member lengths came directly from the given dimensions, while I used the Pythagorean theorem to determine the diagonal member lengths.

<img width="815" height="426" alt="image" src="https://github.com/user-attachments/assets/9439f4ed-4a99-4c9a-9fd1-1d2d08e81c5d" />


| Member | Length |
|---|---:|
| BE | 0.400 m |
| EF | 0.400 m |
| FA | 0.400 m |
| BC | 0.500 m |
| EC | 0.300 m |
| CD | 0.400 m |
| FD | 0.300 m |
| DA | 0.500 m |
| ED | 0.500 m |

The total length of all nine members is:

<p align="center">
L<sub>total</sub> = 3.7 m
</p>

I calculated the total member length because it is later used to estimate the total material volume and weight of the truss.

---

## Overall Free Body Diagram

After determining the dimensions of my truss, I created a free body diagram of the entire structure so I could identify the external forces and solve for the support reactions.

Point A is a pin support, so it can have reaction forces in both the x and y directions. Point B is a roller support and therefore only has a vertical reaction force. The two applied loads of `P = 24 kN` act downward at joints C and D.

<img width="762" height="269" alt="image" src="https://github.com/user-attachments/assets/8766eb2b-5a5c-4b0b-afd9-1c754bff573a" />


### Unknown Support Reactions

- A<sub>x</sub>
- A<sub>y</sub>
- B<sub>y</sub>

<img width="789" height="871" alt="image" src="https://github.com/user-attachments/assets/1b371ccd-41d6-4fa9-9fd7-448ad72d2d64" />

---

## Joint Free Body Diagrams

After solving for the support reactions of the entire truss, I separated the structure into individual joints. Drawing a free body diagram for each joint made it easier to identify the member forces acting at each connection and allowed me to use the equilibrium equations to solve for the internal forces.

I initially assumed that all unknown member forces were in tension, meaning the force arrows pointed away from each joint. If a calculated force was negative, that indicated that the member was actually in compression.

<img width="907" height="600" alt="image" src="https://github.com/user-attachments/assets/7291a671-e0d1-4883-a3f4-e2db86367c18" />

---

## Symbolic Internal Force Calculations

After drawing the free body diagram for each joint, I used the Method of Joints to solve for the internal force in each truss member.

For the symbolic calculations, I kept the applied load as `P` and the truss dimensions as `a` and `b` instead of immediately substituting numerical values. A positive answer represented tension and a negative answer represented compression.

<img width="914" height="2586" alt="image" src="https://github.com/user-attachments/assets/342152a5-127b-4db6-882d-8dd4856514b2" />


---

## Numerical Internal Force Calculations

After solving for the internal member forces symbolically, I substituted my selected load of `P = 24 kN` and the given dimensions of `a = 0.4 m` and `b = 0.3 m`.

<img width="934" height="1954" alt="image" src="https://github.com/user-attachments/assets/13611654-dcb5-4d7f-8b45-bcebf20a212f" />


The resulting member forces were:

| Member | Force | Type |
|---|---:|---|
| BC | 40 kN | Tension |
| BE | 32 kN | Compression |
| EC | 0 kN | Zero-force |
| CD | 32 kN | Tension |
| ED | 0 kN | Zero-force |
| EF | 32 kN | Compression |
| FD | 0 kN | Zero-force |
| DA | 40 kN | Tension |
| FA | 32 kN | Compression |

Members BC and DA experience the largest internal force, with each carrying **40 kN in tension**. The largest compression force is **32 kN** and occurs in members BE, EF, and FA.

Since 40 kN is the largest force magnitude in the truss, I used this value to determine the minimum required cross-sectional area of the members.

---

# Step 2: Truss Member Cross-Sectional Area

## Knowns and Unknowns

After calculating the internal forces in each truss member, I found that the largest force magnitude is 40 kN and occurs in members BC and DA.

Since every truss member is required to have the same cross-sectional area, I used this maximum force to determine the required area for every member.

<img width="782" height="404" alt="image" src="https://github.com/user-attachments/assets/5fc353ff-ace2-4ebf-84df-e896c6e938a0" />


---

## Symbolic Area Calculation

To determine the minimum required cross-sectional area of the truss members, I used the normal stress relationship and the required safety factor.
<img width="693" height="652" alt="image" src="https://github.com/user-attachments/assets/93957ff4-45f4-4f0b-9247-fe00c13c3ff4" />


---

## Numerical Area Calculation

After solving for the minimum cross-sectional area symbolically, I substituted the largest internal force, safety factor, and assumed yield strength into the equation.

<img width="889" height="336" alt="image" src="https://github.com/user-attachments/assets/4f7dd163-f7c5-49d6-8559-6a8c910a8ebf" />


The calculated minimum cross-sectional area was:

<p align="center">
A<sub>min</sub> = 119.4 mm²
</p>

For the CAD model, I selected a rectangular cross section of:

<p align="center">
12 mm × 10 mm
</p>

which gives:

<p align="center">
A = (12)(10) = 120 mm²
</p>

Since:

<p align="center">
120 mm² > 119.4 mm²
</p>

the selected CAD cross-sectional area is slightly larger than the calculated minimum.

---

## Approximate Truss Weight

After determining the minimum cross-sectional area of the truss members, I estimated the total weight of the truss.

Since every member has the same cross-sectional area, I multiplied the area by the total member length to determine the approximate material volume. I then used the assumed steel density to estimate the mass and weight of the truss.

<img width="749" height="575" alt="image" src="https://github.com/user-attachments/assets/5e2a7fb5-a220-46c3-9e0a-a9a168f7fa33" />


Based on these calculations, the approximate hand-calculated weight of the truss is:

<p align="center">
W<sub>truss</sub> ≈ 33.4 N
</p>

This value is later compared with the weight predicted by the Creo CAD model.

---

# Step 3: Pin Design

## Knowns and Unknowns

After determining the required size and approximate weight of the truss members, I moved on to designing the connecting pins.

The pins are made from hardened tool steel and are required to use a single-shear connection with a safety factor of 4.

<img width="844" height="535" alt="image" src="https://github.com/user-attachments/assets/b0ab7ecf-673c-4181-af47-9c7c88e4aa41" />


---

## Critical Pin FBD

The support reactions at A and B are equal, with each having a reaction magnitude of 24 kN. Since both supports experience the same reaction magnitude, either support pin can be used for the critical pin calculation.

I selected pin A and created a free body diagram showing the force acting on the pin in a single-shear connection.

<img width="743" height="398" alt="image" src="https://github.com/user-attachments/assets/fa4aca39-a0d9-4337-bd53-e05b089f162b" />


---

## Symbolic Pin Area Calculation

To determine the minimum required cross-sectional area of the pin, I used the shear stress equation and the required pin safety factor.


<img width="808" height="644" alt="image" src="https://github.com/user-attachments/assets/08be9f1e-4005-439e-a739-5dfdc7ec6116" />

For a circular pin:

<p align="center">
A = πd²/4
</p>

---

## Numerical Pin Area Calculation

After solving for the minimum pin area symbolically, I substituted the maximum pin force of 24 kN, a safety factor of 4, and the hardened tool-steel shear yield strength of 170 ksi.

<img width="918" height="470" alt="image" src="https://github.com/user-attachments/assets/e6428246-2ddd-48f0-b32c-fe9bb2d914bf" />


The minimum required pin area was:

<p align="center">
A<sub>pin,min</sub> ≈ 81.9 mm²
</p>

This corresponds to a minimum pin diameter of approximately:

<p align="center">
d<sub>min</sub> ≈ 10.2 mm
</p>

For the CAD model, I selected:

<p align="center">
d<sub>pin</sub> = 11 mm
</p>

This gives a pin diameter slightly larger than the theoretical minimum.

---

## Approximate Pin Weight

After determining the minimum required cross-sectional area and diameter of the pins, I estimated the combined weight of all six pins.

Since the assignment does not specify a pin length, I assumed each pin has a length of:

<p align="center">
L<sub>pin</sub> = 20 mm
</p>

I used the same 20 mm length in the CAD model so that the hand calculation and CAD results could be compared consistently.

<img width="907" height="832" alt="image" src="https://github.com/user-attachments/assets/1ddfc400-128a-4efd-bdc3-68748f329352" />


Based on the hand calculations, the approximate combined weight of all six pins is:

<p align="center">
W<sub>pins</sub> ≈ 0.167 lb
</p>

---

# Step 4: CAD Model

After completing my hand calculations, I created a 3D model of the truss in Creo 13. I used the same geometry and dimensions from my statics calculations and designed the truss members to meet the required cross-sectional area.

I modeled the truss without the pins as one part and added additional material around each joint so that the required cross-sectional area would be maintained after the pin holes were created.

---

## CAD Design Process

I first created a 2D sketch of the truss geometry using the dimensions from my hand calculations. The horizontal spacing between joints was set to 400 mm and the vertical distance was set to 300 mm.

This sketch provided the centerline paths used to create the individual truss members.

<img width="939" height="498" alt="image" src="https://github.com/user-attachments/assets/d5a052bb-6997-4d02-b4a7-e22cbb77dc0e" />


This screenshot shows the initial 2D truss layout in Creo before any solid geometry was created. I kept the same geometry and dimensions that were used in my hand calculations.

I then used the Sweep feature in Creo to create solid truss members along the paths of the original sketch.

Each member was given the same rectangular cross section:

<p align="center">
12 mm × 10 mm
</p>

giving:

<p align="center">
A = 120 mm²
</p>

This is slightly larger than the calculated minimum area of 119.4 mm².

<img width="936" height="493" alt="image" src="https://github.com/user-attachments/assets/2a7c942d-5fc7-4e43-a543-f08ecd5ed196" />


After creating the centerline sketch, I used the Sweep feature to turn the sketch paths into solid truss members. All members were created with the same cross-sectional dimensions so that the CAD model remained consistent with the assumptions used in my calculations.

---

### Reinforced Pin Joints

Before creating the pin holes, I added circular joint areas at all six connection points.

Each joint pad was modeled with:

- Outer diameter = 25 mm
- Thickness = 10 mm

<img width="930" height="489" alt="image" src="https://github.com/user-attachments/assets/76599b7e-3b2d-40f5-ba3e-c4fc8604cac1" />


The larger joint areas provide additional material around the pin locations so that creating the holes does not remove too much material from the members.

The remaining width through the center of the joint after creating an 11 mm hole is:

<p align="center">
25 mm - 11 mm = 14 mm
</p>

Therefore, the approximate remaining cross-sectional area through the joint is:

<p align="center">
A<sub>joint</sub> = (14)(10)
</p>

<p align="center">
A<sub>joint</sub> = 140 mm²
</p>

Since:

<p align="center">
140 mm² > 120 mm²
</p>

the joint maintains at least the same cross-sectional area as the regular truss members.

<img width="933" height="492" alt="image" src="https://github.com/user-attachments/assets/02fc8e94-2ee6-4b7e-a9a1-b877397c2b7e" />


After reinforcing all six joints, I created an **11 mm diameter hole** through each joint. I selected 11 mm because the calculated minimum pin diameter was approximately 10.2 mm.

This completed the truss portion of the CAD model before the pins were added.

---

## Material and Mass Properties

The exact materials specified in the assignment were not available in the Creo material library.

The truss was required to use **A500 structural steel**, so I selected **Low Carbon Steel** as the closest available material for the CAD mass calculation.

The pins were required to use **hardened tool steel**, so I selected **Air-Hardening Tool Steel** from the Creo material library.

Because the Creo material properties and densities are slightly different from the values used in my hand calculations, I expected the CAD weight to be close to, but not exactly the same as, my calculated value.

<img width="930" height="523" alt="image" src="https://github.com/user-attachments/assets/503cea99-ba29-4a33-bea9-af0b59ae8192" />


I used Creo's material properties tools to assign the appropriate material to each part of the model. This allowed Creo to use the modeled geometry and assigned material density to calculate the predicted mass.

---

### Pin Material

For the pins, I selected **Air-Hardening Tool Steel** because it was the closest available Creo material to the hardened tool steel specified in the assignment.

Creo lists a density of approximately:

<p align="center">
0.284 lb/in³
</p>

while the assignment specifies:

<p align="center">
0.278 lb/in³
</p>

This small difference in density contributes to the difference between the hand-calculated and CAD pin weights.

<img width="938" height="746" alt="image" src="https://github.com/user-attachments/assets/d3b93c64-6fc3-4278-8ab9-8cfbce76b747" />


---

### Pin Mass Properties

After assigning the pin material, I used Creo's Mass Properties tool to determine the mass of one pin.

The CAD pin was modeled using:

- Diameter = 11 mm
- Length = 20 mm

Creo calculated a mass of:

<p align="center">
1.4939 × 10⁻⁵ tonne
</p>

Converting this value to pounds-mass:

<p align="center">
0.0329 lbm per pin
</p>

<img width="934" height="531" alt="image" src="https://github.com/user-attachments/assets/0adc30ec-f5bc-429a-a156-cc4c33329eb0" />


This screenshot verifies the final pin dimensions used in the CAD model. The 11 mm pin diameter is slightly larger than the calculated minimum diameter of 10.2 mm, while the 20 mm length matches the assumed length used in the hand calculations.

<img width="940" height="527" alt="image" src="https://github.com/user-attachments/assets/de0fa7a3-a5bc-4106-83e4-e7f3f2d9df3b" />


---

## Truss Assembly

I created a Creo assembly using the completed truss part and the pin part.

I first aligned the cylindrical surface of each pin with the cylindrical surface of the corresponding joint hole so that the pin axis was centered with the hole.

<img width="938" height="532" alt="image" src="https://github.com/user-attachments/assets/1f8ef461-7c33-4f4f-969c-ffc055d73603" />


After aligning the pin with the hole, I added a second coincident constraint between the flat end of the pin and the face of the truss joint.

This fully constrained the pin and controlled its position through the thickness of the truss.

<img width="934" height="526" alt="image" src="https://github.com/user-attachments/assets/553d7a97-31a0-4402-857f-0e3ac1936447" />


I repeated this process until all six identical pins were positioned at the six truss joints.

The completed assembly contains:

- 1 truss part
- 6 identical pin parts

<img width="934" height="529" alt="image" src="https://github.com/user-attachments/assets/9bde245e-0555-46d9-876a-7d41a3ce1071" />


This completed assembly represents the final geometry used for the CAD mass-properties calculation.

---

## Final CAD Mass Properties

After assigning materials to both the truss and pins, I used Creo's Mass Properties tool to calculate the predicted mass of the complete assembly.

<img width="939" height="528" alt="image" src="https://github.com/user-attachments/assets/436b02a9-6cda-4845-9d13-5fc778c37389" />


Creo predicted:

| Component | CAD Mass |
|---|---:|
| Truss | 7.641 lbm |
| Six pins | 0.198 lbm |
| Complete assembly | **7.839 lbm** |

The complete assembly mass corresponds to a weight of approximately:

<p align="center">
W<sub>CAD</sub> ≈ 34.87 N
</p>

---

## Hand Calculation vs. CAD Weight

My hand calculations predicted a truss weight of approximately **33.4 N** and a combined pin weight of approximately **0.167 lb**.

This gives a total hand-calculated weight of approximately:

<p align="center">
W<sub>hand</sub> ≈ 34.14 N
</p>

The completed Creo model predicted:

<p align="center">
W<sub>CAD</sub> ≈ 34.87 N
</p>

The percent difference is:

<p align="center">
Percent Difference = ((34.87 - 34.14) / 34.14)(100)
</p>

<p align="center">
Percent Difference ≈ 2.1%
</p>

The Creo model is approximately **2.1% heavier** than my hand calculation.

This difference is reasonable because the CAD model includes additional material around the pin joints, uses an actual pin diameter of 11 mm rather than the exact calculated minimum diameter, and uses Creo material properties that are slightly different from the densities used in my hand calculations.

---

# Engineering Lessons Learned

This assignment helped me better understand how statics calculations connect to an actual engineering design. I learned that the internal member forces determine the required cross-sectional area, while the forces at the connections determine the required pin size.

I also learned that a design that works mathematically still needs to be adjusted when creating the CAD model. For example, I added material around the pin holes and selected member and pin dimensions that were slightly larger than the calculated minimum values.

Comparing my hand calculations with the Creo mass properties also showed me why analytical and CAD results may be slightly different. Small changes in geometry, selected dimensions, and material properties can affect the predicted weight of the final design.

---
# 2157 Additional Analysis: Failure Modes

## Part 1 – Truss Members

For this part, I looked at the different ways that the members of my truss could fail. The members are either in tension, compression, or are zero-force members. The type of force in each member helped me determine which failure mode would be the most likely.

The truss was designed using A500 structural steel. A500 steel is a ductile material, meaning that it will normally start to deform or yield before completely breaking.

### Member Stress

I used the internal forces that I calculated earlier and the cross-sectional area of my CAD members to compare the stress in each member.

The cross-sectional area of each member is:

<p align="center">
A = 12 mm × 10 mm = 120 mm²
</p>

I calculated the normal stress using:

<p align="center">
σ = F / A
</p>

| Member | Force | Type | Stress | Expected Failure |
|---|---:|---|---:|---|
| BC | 40 kN | Tension | 333 MPa | Yielding |
| BE | 32 kN | Compression | 267 MPa | Buckling |
| EC | 0 kN | Zero Force | 0 MPa | None |
| CD | 32 kN | Tension | 267 MPa | Yielding |
| ED | 0 kN | Zero Force | 0 MPa | None |
| EF | 32 kN | Compression | 267 MPa | Buckling |
| FD | 0 kN | Zero Force | 0 MPa | None |
| DA | 40 kN | Tension | 333 MPa | Yielding |
| FA | 32 kN | Compression | 267 MPa | Buckling |

### Tension Members

Members **BC, CD, and DA** are in tension. BC and DA have the largest tensile force at 40 kN, which gives them a stress of about 333 MPa. CD has a smaller force of 32 kN and a stress of about 267 MPa.

The most likely failure for these members would be yielding. Since the steel is ductile, I would expect it to start permanently deforming before it completely fractures. BC and DA would be the most concerning because they have the highest tensile stress.

One way I could make these members less likely to fail would be to increase their cross-sectional area. This would lower the stress in the members because the same force would be spread over a larger area.

### Compression Members

Members **BE, EF, and FA** are in compression. Each of these members has a force of about 32 kN and a normal stress of about 267 MPa.

The failure mode I would be most concerned about for these members is buckling. A long member under compression can bend sideways and become unstable instead of simply being crushed.

One way I could reduce the chance of buckling would be to make the members thicker or use a cross section that is more resistant to bending. Adding more support to shorten the unsupported length could also help.

### Zero-Force Members

Members **EC, ED, and FD** had a calculated internal force of approximately zero for this loading condition. Because of this, they have essentially no normal stress and are not expected to fail under the current loading.

Even though they are zero-force members for this situation, I would still keep them in the design because they help maintain the shape and stability of the truss and could carry forces if the loading changed.


## Part 2 – Pin Connections

The pins in my truss were designed as single-shear connections. Based on this, the failure mode I would be most concerned about is shear failure through the pin.

My final CAD pin has:

- Diameter = 11 mm
- Length = 20 mm
- Maximum pin force = 24 kN

The cross-sectional area of the pin is:

<p align="center">
A = πd² / 4
</p>

<p align="center">
A ≈ 95.0 mm²
</p>

I then calculated the shear stress:

<p align="center">
τ = V / A
</p>

<p align="center">
τ ≈ 253 MPa ≈ 36.6 ksi
</p>

The assignment gives the hardened tool steel pins a shear yield strength of **170 ksi** and requires a safety factor of 4.

Therefore, the allowable shear stress is:

<p align="center">
τ_allow = 170 ksi / 4 = 42.5 ksi
</p>

My calculated pin stress was about **36.6 ksi**, which is below the allowable value of **42.5 ksi**. This means that my 11 mm pin meets the required safety factor based on the shear calculation.

If I wanted to make the pin less likely to fail, I could increase the diameter. A larger diameter would give the pin more cross-sectional area and lower the shear stress.


## Failure Mode Summary

| Component | Expected Failure | Why | Possible Improvement |
|---|---|---|---|
| BC | Yielding | High tension | Increase member area |
| BE | Buckling | Compression | Increase member stiffness |
| EC | None | Zero-force member | Keep for stability |
| CD | Yielding | Tension | Increase member area |
| ED | None | Zero-force member | Keep for stability |
| EF | Buckling | Compression | Increase member stiffness |
| FD | None | Zero-force member | Keep for stability |
| DA | Yielding | High tension | Increase member area |
| FA | Buckling | Compression | Increase member stiffness |
| Pins | Shear failure | Single-shear connection | Increase pin diameter |


## Sources

- Steel Tube Institute, *ASTM A500*
- American Institute of Steel Construction (AISC), *Fundamentals of Structural Stability for Steel Design*
- Purdue University ME 323, *Shear Stress and Shear Strain*

## AI Use

I used AI to help make my portfolio look better and improve the formatting. I asked AI how to **bold certain words**, **center text**, and **make a chart/table in GitHub Markdown**. I used the responses as a guide when formatting my portfolio.
<p align="center">
  <img src="https://github.com/user-attachments/assets/e9f4e4ee-f534-47d3-98ad-7c7e85ab0370" width="30%" />
  <img src="https://github.com/user-attachments/assets/8fcb1726-2a26-4412-90c2-e954533a09a7" width="30%" />
  <img src="https://github.com/user-attachments/assets/d10b0b05-1c7f-409b-9d13-003646bde3a3" width="30%" />
</p>


# Time Spent

I spent approximately **18 hours** completing this assignment. The CAD model and documentation took the most time because I had to make several adjustments while creating the truss, joints, pins, and assembly in Creo.

I also spent additional time organizing my calculations and screenshots so that the complete engineering design process was clearly documented and looked organized in my portfolio.

---

# CAD File Download

[A2_Truss_Creo_Files.zip](https://github.com/user-attachments/files/31771822/A2_Truss_Creo_Files.zip)


## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

I chose a triangular truss design because triangles help make the truss stable and keep it from changing shape when a load is applied. I also chose this design because it was fairly simple while still spreading the forces between multiple members. Overall, I thought it would give me a strong and lightweight truss without making the design too complicated.


## Communicate

