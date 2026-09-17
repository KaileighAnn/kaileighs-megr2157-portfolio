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

### Design for Strength

The first design approach is based on the yield strength of PLA. The maximum bending moment occurs at the fixed end of the cantilever beam.


### Strength Calculations

The strength analysis was completed using the bending stress equation and a safety factor of 3. My symbolic and numerical calculations are shown below.

<img width="836" height="1090" alt="image" src="https://github.com/user-attachments/assets/53c5255b-f324-4d19-a4d9-b0579caa3be1" />


The minimum required height based on strength was:

**h = 9.49 mm**


### Design for Deflection

The second approach was based on limiting the maximum deflection of Feature 1 to **0.30 mm**. My symbolic and numerical calculations are shown below.

PIC

The minimum required height based on deflection was:

**h = 10.63 mm**


### Feature 1 Results

The two calculated dimensions for Feature 1 were:

- **Strength: 9.49 mm**
- **Deflection: 10.63 mm**

Since the deflection analysis required the larger dimension, deflection controlled the design. I rounded the calculated value of 10.63 mm up and selected a final dimension of:

**h = 11 mm**


## Feature 2

Feature 2 is the portion of the motor mount that attaches to the rigid wall. The wall was assumed to be rigid and capable of supporting the mounting bolts. Feature 2 was analyzed using the same beam bending approach as Feature 1.

### Knowns and Unknowns

#### Knowns

- Applied force: **P = 300 N**
- Length: **L = 30 mm**
- Safety factor: **N = 3**
- Maximum allowable deflection: **0.30 mm**
- Elastic modulus: **E = 3000 MPa**
- Yield strength: **60 MPa**
- Allowable stress: **20 MPa**
- Motor weight is neglected

#### Unknowns

- Required dimension based on strength
- Required dimension based on deflection
- Final dimension of Feature 2


### Feature 2 Free Body Diagram

The free body diagram below shows the simplified beam model used for Feature 2.

<img width="607" height="284" alt="image" src="https://github.com/user-attachments/assets/5a4fce24-8ed0-44c7-897a-e325ed876790" />

### Feature 2 Calculations

Feature 2 was analyzed using the same beam bending and deflection equations used for Feature 1. My calculations are shown below.

<img width="849" height="408" alt="image" src="https://github.com/user-attachments/assets/c43722dc-e35e-40b7-8052-f5faae4e2604" />


The deflection calculation resulted in a required dimension of approximately:

**h = 9.576 mm**

I rounded this value up and selected a final dimension of:

**h = 10 mm**


### Feature 2 Results

The calculated dimensions were used to determine the final geometry of Feature 2. The final dimension selected for the CAD model was:

**h = 10 mm**

# Motor Mount Design

After completing the calculations for both features, I used the calculated dimensions to create the motor mount in SolidWorks. The design was developed around the dimensions of the selected motor while also including the required wall mounting surface and clearance holes.

## Initial Motor Mount Design

I first created the main mounting geometry and added the opening for the motor and shaft. The two mounting surfaces were positioned perpendicular to each other to create the basic shape of the motor mount.

<img width="957" height="600" alt="Screenshot 2026-09-16 224741" src="https://github.com/user-attachments/assets/7aaa9df1-4919-42ac-b6da-a44b6e713728" />

## Wall Mounting Feature

I then added the wall mounting portion of the design. Four clearance holes were added to provide attachment points between the motor mount and the rigid wall.

<img width="1913" height="1200" alt="Screenshot 2026-09-16 225758" src="https://github.com/user-attachments/assets/861bbd6e-7c7e-4e23-8735-6b859752319f" />

## Final Motor Mount Design

The final design combines the motor mounting feature and wall mounting feature into a single part. The motor is positioned within the main mounting area, while the second surface provides the connection to the rigid wall.

The final model includes the motor and shaft clearance, four wall mounting holes, and the dimensions determined from my beam calculations.

<img width="1914" height="1200" alt="Screenshot 2026-09-16 230951" src="https://github.com/user-attachments/assets/b7b57163-be57-4754-831b-9cae475da33a" />


## Motor Mount Research

Before creating my final design, I looked at different motor mount designs to get an idea of common mounting methods and ways to make the mount more rigid.

Some of the features I considered were:

- L-shaped mounting geometry
- Flat surfaces for mounting the motor and attaching to the wall
- Clearance for the motor and shaft
- Multiple mounting holes
- Additional material around the corners to increase rigidity

The links I used for design inspiration are included in the Appendix.


## Isometric Sketch

After completing the calculations for both features, I created an isometric sketch of my motor mount. The calculated dimensions were used to help determine the overall size and shape of the design.

<img width="449" height="319" alt="image" src="https://github.com/user-attachments/assets/6185e179-e58c-46f1-9e5c-0b0da4a82ef5" />


## CAD File

The final SolidWorks CAD file can be downloaded below.

[Download A04 Motor Mount CAD File](...)
 

## Parametric Modeling

I created the final motor mount in SolidWorks using the dimensions determined from my calculations. I used parametric dimensions where appropriate so that important dimensions could be changed without completely rebuilding the model.

Important dimensions used in the final design included:

- **Motor mounting width: 30 mm**
- **Feature 1 thickness: 11 mm**
- **Feature 2 thickness: 10 mm**
- **Motor clearance: approximately 28 mm**
- **Shaft clearance: 6 mm**
- **Wall mounting holes: 3.4 mm**


## Initial CAD Model

I started by creating the basic geometry for the motor mounting feature using the dimensions determined from my calculations.

PIC


## Motor and Shaft Clearance

Next, I added clearance for the motor and motor shaft. The motor dimensions were used to make sure the motor could fit correctly within the mount.

PIC


## Wall Mounting Feature

The second feature was then added to create the wall mounting portion of the design.

Four **3.4 mm clearance holes** were added for the mounting bolts.

PIC


## Design Features to Minimize Deflection

The dimensions determined from the deflection calculations were used as minimum dimensions for the final design.

Instead of using the exact calculated values, I rounded the dimensions upward. Feature 1 was increased from **10.63 mm to 11 mm**, and Feature 2 was increased from approximately **9.576 mm to 10 mm**.

I also kept additional material around the mounting surfaces and corners to increase the rigidity of the mount and help reduce deflection.


## Final CAD Model

After completing both mounting features and adding all required clearance holes, I completed the final motor mount.

PIC


## CAD File

The final SolidWorks CAD file can be downloaded below.

**[Download Motor Mount CAD File](ADD CAD FILE LINK HERE)**


# Engineering Drawing

## Multiview Drawing

After completing the 3D CAD model, I created a multiview engineering drawing of the motor mount.

The drawing includes:

- Front View
- Right Side View
- Top View
- Isometric View
- Size and location dimensions
- Hole callouts
- Center marks and centerlines
- Third-angle projection
- Title block
- Material and scale

The drawing was dimensioned to clearly communicate the geometry of the final motor mount.


## Final Engineering Drawing

PIC


# Mistakes and Changes

One of the main changes I made during the design process was rounding my calculated dimensions to practical dimensions for CAD. Feature 1 required a minimum dimension of **10.63 mm**, so I increased it to **11 mm**. Feature 2 required approximately **9.576 mm**, so I increased it to **10 mm**.

I also made adjustments while creating the CAD model to make sure the motor clearance, shaft hole, mounting holes, and overall geometry fit together correctly.


# Lessons Learned

This assignment helped me understand how beam calculations can be used to determine actual dimensions before creating a part in CAD. I also learned that designing for strength does not necessarily mean that the design will meet the deflection requirement. For Feature 1, deflection controlled the final dimension because it required a larger cross section than the strength calculation.

I also learned how useful parametric modeling can be when dimensions need to be adjusted during the design process. Using the calculated values as the starting point helped connect the engineering analysis directly to the final CAD model.


# Time Spent

- Calculations: **___ hours**
- Research and sketching: **___ hours**
- CAD modeling: **___ hours**
- Engineering drawing: **___ hours**
- Portfolio documentation: **___ hours**

**Total Time: ___ hours**


# Appendix

## Motor Mount Research Links

1. [Motor Mount Design Inspiration 1](ADD LINK HERE)
2. [Motor Mount Design Inspiration 2](ADD LINK HERE)
3. [Motor Mount Design Inspiration 3](ADD LINK HERE)


## Motor Information

The motor used for this assignment was the **Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM with 99.5:1 Planetary Gearbox**.

[Motor Specifications](https://www.omc-stepperonline.com/brushed-24v-dc-gear-motor-3-6kg-cm-46rpm-w-99-5-1-planetary-gearbox-pa28-28245800-g100)
