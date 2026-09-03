# A2 – Truss Stress Analysis

## Objective


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



