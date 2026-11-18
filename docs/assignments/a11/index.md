# A11 – Motor Selection

## Motor Selection and Calculations -- Kelsey Skipper

## Objective

My objective for this assignment was to perform the engineering calculations necessary to support the design of the mechanical tensile tester. This included motor and material selection, motor mount bearing stress analysis, coupler torsional stress analysis, frame reaction force calculations, and floating bearing fit tolerances. I also established the loading conditions for my teammates' finite element analyses and updated the bill of materials. These calculations were performed to evaluate the design's ability to withstand a maximum tensile load of 2 kN while maintaining a minimum factor of safety of 4.

## Analyze

### Design Parameters

Using the calculations completed in Part 1, I established the following design parameters:

| Parameter | Value |
|---|---:|
| Maximum tensile load | 2,000 N |
| Load per leadscrew | 1,000 N |
| Factor of safety | 4 |
| Leadscrew diameter | 3/8 in |
| Leadscrew length | 24 in |
| Thread specification | 3/8-12 ACME |
| Operational torque | 4.759 N·m |
| Required design torque | 19.036 N·m |
| Rotational speed | 0.473–23.62 RPM |

### Motor Selection

I selected two McMaster-Carr DC gearmotors (6470K84), one for each leadscrew. Each motor has a listed rated torque of 24.857 N·m and a rated speed of 31 RPM. The rated torque exceeds the calculated design torque requirement. Low-speed operation and the complete torque-speed relationship require further verification.

<img width="3094" height="4641" alt="IMG_7871" src="https://github.com/user-attachments/assets/9a6996eb-44a8-4d83-a464-82720e6b1d81" />

<img width="377" height="284" alt="Screenshot 2026-11-16 214242" src="https://github.com/user-attachments/assets/bc217370-819a-4948-9e19-d67b5a2ef96b" />

### Motor Mount

I selected Aluminum 6061-T6 for the motor mounts due to its strength, low weight, and machinability. I analyzed the reaction forces acting on the mounting bolts and calculated the minimum plate thickness based on allowable bearing stress.

<img width="3641" height="3134" alt="IMG_7872" src="https://github.com/user-attachments/assets/e4f8e94c-af0f-4362-a341-dde0a9757f14" />

### Coupler

I analyzed the coupler using torsional shear stress equations to determine the minimum outer diameter and wall thickness. Aluminum 6061-T6 was selected as the coupler material. The motor-side bore must accommodate the selected motor's 15.875 mm output shaft.

<img width="3504" height="4484" alt="IMG_7873" src="https://github.com/user-attachments/assets/32f3199c-6238-4d86-8980-e942582fc552" />

### Frame Connectors

I calculated the vertical and transverse reaction forces acting on the frame connectors due to the axial loads and motor reaction moments. These forces were used to determine the stresses acting on the connectors and evaluate their required thickness.

<img width="3340" height="4556" alt="IMG_7874" src="https://github.com/user-attachments/assets/6c29c214-e570-498b-801e-90fa1341909e" />

### Horizontal Frame Analysis

The horizontal frame consists of heavy 40 Series aluminum T-slot extrusion. The loading conditions for the finite element analysis consist of two 1,000 N axial loads and two motor reaction moments of approximately 25 N·m.

<img width="3709" height="3083" alt="IMG_7875" src="https://github.com/user-attachments/assets/257fe632-75c8-437f-8d8d-da1577e5486e" />

### Vertical Frame Analysis

The vertical frame members were analyzed under axial compression and transverse loading resulting from the motor reaction moments. The objective of the analysis was to verify that the frame maintains a minimum factor of safety of 4.

<img width="3796" height="3391" alt="IMG_7876" src="https://github.com/user-attachments/assets/d7c3873f-7bf6-4ed2-9c3e-936bf32fc5ed" />

### Floating Bearing Mount

I selected an RC3 running fit for the floating bearing interface to allow rotation without excessive clearance. I determined the shaft and hole tolerances, minimum and maximum clearances, and mounting bolt clearance requirements.

<img width="1985" height="4967" alt="IMG_7877" src="https://github.com/user-attachments/assets/bb661d98-5aed-4e39-83a1-99564ad583f8" />

<img width="2101" height="2043" alt="IMG_7878" src="https://github.com/user-attachments/assets/ef7e0db4-5df1-47b1-be97-cb71e951ad53" />

## Decide

Based on the preliminary engineering calculations, the following components and materials were selected:

| Component | Selection |
|---|---|
| Motors | McMaster-Carr 6470K84 |
| Leadscrews | 1080 carbon steel |
| Leadscrew nuts | SAE 932 bearing bronze |
| Motor mounts | Aluminum 6061-T6 |
| Couplers | Aluminum 6061-T6 |
| Frame connectors | Aluminum 6061-T6 |
| Horizontal frame | Heavy 40 Series aluminum extrusion |
| Vertical frame | Heavy 40 Series aluminum extrusion |
| Floating bearing mounts | Aluminum 6061-T6 |
| Fasteners | Steel |

These selections were made based on strength, machinability, availability, and compatibility with the existing assembly. Final verification is dependent on the FEA results, actual component dimensions, motor operating characteristics, and leadscrew capacity.

## Communicate

### Bill of Materials

| Component | Qty. | Unit Cost | Total | Supplier |
|---|---:|---:|---:|---|
| 3/8"-12 Acme Lead Screw | 2 | $35.32 | $70.64 | [McMaster-Carr](https://www.mcmaster.com/99030A993/) |
| Bronze Flange Nut | 2 | $111.78 | $223.56 | [McMaster-Carr](https://www.mcmaster.com/95120A592/) |
| DC Gearmotor | 2 | $500.00* | $1,000.00 | [McMaster-Carr](https://www.mcmaster.com/6470K84/) |
| Thrust Bearing | 2 | $25.00* | $50.00 | [McMaster-Carr](https://www.mcmaster.com/thrust-bearings/) |
| Bronze Bushing | 2 | $5.00* | $10.00 | [McMaster-Carr](https://www.mcmaster.com/bushings/) |
| Assorted Mounting Hardware | 1 set | $40.00* | $40.00 | [McMaster-Carr](https://www.mcmaster.com/) |
| **Total** | | | **$1,394.20** | |

*Prices marked with an asterisk are estimated and subject to supplier verification.*

### Lessons Learned

Through this assignment, I learned how motor torque influences the design of mechanical components and supporting structures. I also gained a better understanding of bearing tolerances, torsional loading, and how hand calculations can be used alongside FEA to evaluate a mechanical system. Additionally, I learned the importance of verifying purchased component specifications before finalizing a design.

### Time Spent
The total time spent on my portion of this assignment was roughly 5 hours to complete all of the calculations and select the motor.

## FEA - Gracie Steelmon

For this assignment I started by taking Kelseys calculations for the mounting bracket and designing it in Solidworks. Once I had that completed I opened up our previous CAD model from A10 and started to assemble. 

<img width="2101" height="2043" alt="<img width="767" height="322" alt="Screenshot 2026-11-17 105937" src="https://github.com/user-attachments/assets/a1085504-8fa4-4a4e-b3ba-a5e19ddcca66" />

Once I had the bracket on I then needed to decide on screws and nuts to use. The diameter of the hole was 6.6mm which is roughly 0.259843 inches. The screw I selected was a M4 x 0.7mm. This screw seemed more fit for a 6.6mm hole. Especially if this was the minimum diameter. For the length I added the thickness of the motor mount and the thickness of the cross head to become around 2.07 inches. From there I selected the 70mm long screw. This was the excess left over on the bottom can ensure that the nut will have enough length to fit and any vibrations will not cause things to fall apart. These are made out of 18-8 stainless steel. 

<img width="886" height="388" alt="image" src="https://github.com/user-attachments/assets/1571c766-708f-41bd-84e3-2383c41fd2ae" />
<img width="751" height="310" alt="image" src="https://github.com/user-attachments/assets/3fbd0ece-8c9d-4f42-b50b-8665ed00ff3d" />
<img width="793" height="380" alt="Screenshot 2026-11-17 105946" src="https://github.com/user-attachments/assets/755ec001-5631-436f-96a5-6d5318dd7a6d" />



### Fixed Geometry and Loads
For the fixed geometry I fixed the bottom of the entire bracket down. I did two loads of 1kN each down on the leadscrews. I also applied a torque going the same direction into the holes where the motor will sit at. This torque applied was 24.857 N-M. 
<img width="1242" height="729" alt="Screenshot 2026-11-17 125500 (1)" src="https://github.com/user-attachments/assets/1f53a527-4558-45c3-95c4-e20c1afe05c6" />
<img width="1632" height="885" alt="Screenshot 2026-11-17 130717" src="https://github.com/user-attachments/assets/335c16fd-3642-4dca-b334-5ea432f82544" />

<img width="1465" height="931" alt="Screenshot 2026-11-17 124428 (1)" src="https://github.com/user-attachments/assets/46b9834c-2a4f-4a5f-bfaf-96e327b5e141" />

### Mesh
For the mesh I ran into several problems. I initially tried to create it doing a medium sized mesh and it did not generate correctly other than blowing my computer up. Next I tried the course ones, this did not work either. So I went back to medium size and it worked that time. 

### Results
#### - Von Misses
<img width="1648" height="862" alt="Screenshot 2026-11-17 132749" src="https://github.com/user-attachments/assets/2d898f73-c823-4d27-ada1-fb55e13b7eb8" />

#### - FOS
<img width="1658" height="838" alt="Screenshot 2026-11-17 133239" src="https://github.com/user-attachments/assets/3d213265-15a0-4a0c-88ba-adc5180b6d2d" />

#### - Strain
<img width="1670" height="854" alt="Screenshot 2026-11-17 133032" src="https://github.com/user-attachments/assets/bbbaa978-45cc-4060-aa4f-eca9d73241d7" />


### Alternate Design Suggestions
This FEA did not turn out as bad as I thought. Some design aterations could be to change the material to be stronger. the torque had more effect than the 1kN load did. 

### CAD Files
![](Assem2.zip)


## Bill of Materials and Engineering Drawing Package – Kaileigh Hill

### Objective

My objective for this portion of the assignment was to organize the Bill of Materials (BOM) for both A10 and A11, calculate the total engineering labor costs, and create an engineering drawing package for the tensile tester using SolidWorks.

## Bill of Materials and Labor Costs

### Bill of Materials

The following table includes the components selected for our tensile tester. Costs were taken from our previous assignment, McMaster-Carr, and Grainger.

| Component | Qty. | Unit Cost | Total | Supplier |
|---|---:|---:|---:|---|
| 3/8"-12 Acme Lead Screw | 2 | $35.32 | $70.64 | [McMaster-Carr](https://www.mcmaster.com/99030A993/) |
| Bronze Flange Nut | 2 | $111.78 | $223.56 | [McMaster-Carr](https://www.mcmaster.com/95120A592/) |
| T-Slot Framing | 1 | $245.87 | $245.87 | [Grainger](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48) |
| DC Gearmotor | 2 | $500.00* | $1,000.00 | [McMaster-Carr](https://www.mcmaster.com/6470K84/) |
| Thrust Bearing | 2 | $25.00* | $50.00 | [McMaster-Carr](https://www.mcmaster.com/thrust-bearings/) |
| Bronze Bushing | 2 | $5.00* | $10.00 | [McMaster-Carr](https://www.mcmaster.com/bushings/) |
| M4 x 0.7 mm, 70 mm Screws (Pack of 10) | 1 pack | $12.88 | $12.88 | [McMaster-Carr](https://www.mcmaster.com/92010A819/) |
| M4 x 0.7 mm Hex Nuts (Pack of 4,000) | 1 pack | $85.12 | $85.12 | McMaster-Carr |
| Assorted Mounting Hardware | 1 set | $40.00* | $40.00 | [McMaster-Carr](https://www.mcmaster.com/) |
| **Current Material Subtotal** | | | **$1,738.07** | |

*Prices marked with an asterisk are estimated. Screw and nut prices reflect full package costs.*

The current subtotal includes the components priced so far. Custom-fabricated components, additional frame connectors, and specimen clamps still require cost estimates.

### Engineering Labor Costs

Engineering labor was calculated using the required rate of $35 per hour. This includes the time spent on both A10 and A11.

| Team Member | A10 Hours | A11 Hours | Total Hours | Labor Cost |
|---|---:|---:|---:|---:|
| Kaileigh Hill | 4 | [INSERT] | [INSERT] | [INSERT] |
| Kelsey Skipper | 3 | 5 | 8 | $280.00 |
| Gracie Steelmon | 5 | [INSERT] | [INSERT] | [INSERT] |
| **Total** | **12** | **[INSERT]** | **[INSERT]** | **[INSERT]** |

**Labor Cost = Total Hours × $35/hr**

### Total Engineering Cost

| Category | Cost |
|---|---:|
| Materials Priced So Far | $1,738.07 |
| A10 Engineering Labor | $420.00 |
| A11 Engineering Labor | $[INSERT] |
| Additional Material/Fabrication Costs | $[INSERT] |
| **Total Project Cost** | **$[INSERT]** |

The total project cost includes the material expenses and engineering labor required for both assignments.

---

## Engineering Drawing Package

### Objective

The objective of this portion was to create engineering drawings for the designed tensile tester components and the overall assembly. These drawings document the dimensions, tolerances, and assembly details needed for manufacturing.

### Drawing Standards

All drawings were prepared using third-angle projection and ASME Y14.5 dimensioning and tolerancing standards.

The following general tolerances were used:

| Dimension | Tolerance |
|---|---|
| X.X | ±0.02 in |
| X.XX | ±0.01 in |
| X.XXX | ±0.005 in |

Each drawing includes a title block with the part name, material, scale, and units.

### Component Drawings

#### Crosshead

The crosshead drawing from A10 was included to show the overall dimensions, lead screw openings, and mounting features.

<img src="https://github.com/user-attachments/assets/75371664-f118-46c5-852b-8c5e30228bd8" width="750">

**Figure 1:** Engineering drawing of the crosshead from A10.

#### Motor Mount Bracket

The motor mount drawing shows the bracket dimensions, motor mounting holes, and frame attachment locations.

[INSERT MOTOR MOUNT DRAWING]

**Figure 2:** Engineering drawing of the motor mounting bracket.

#### Motor-to-Leadscrew Coupler

The coupler drawing shows the dimensions and connection features needed to attach the motor shaft to the lead screw.

[INSERT COUPLER DRAWING]

**Figure 3:** Engineering drawing of the motor-to-leadscrew coupler.

#### Floating Bearing Mount

The floating bearing mount drawing includes the mounting hole locations and RC3 fit tolerances.

[INSERT FLOATING BEARING DRAWING]

**Figure 4:** Engineering drawing of the floating bearing mount.

#### Frame Components

The frame drawing shows the heavy 40 Series T-slot framing and connection locations.

[INSERT FRAME DRAWING]

**Figure 5:** Engineering drawing of the frame components.

#### Specimen Clamps

The clamp drawing shows the dimensions and features needed to secure the specimen during testing.

[INSERT CLAMP DRAWING]

**Figure 6:** Engineering drawing of the specimen clamp.

### Complete Assembly Drawing

The assembly drawing shows the tensile tester with the frame, crosshead, motors, lead screws, and other components. The drawing includes an isometric view and a Bill of Materials with corresponding item balloons.

[INSERT ASSEMBLY DRAWING]

**Figure 7:** Isometric engineering drawing of the complete tensile tester assembly.

### Drawing Package and CAD Files

The engineering drawings and SolidWorks CAD files are provided below.

[Download Engineering Drawing Package](INSERT_LINK)

[Download SolidWorks CAD Assembly](https://github.com/user-attachments/files/34669260/Assem2.zip)

---

## Lessons Learned

Through this assignment, I learned how to organize a Bill of Materials and calculate engineering labor costs for a mechanical system. I also learned how to create engineering drawings in SolidWorks and apply dimensions and tolerances to communicate the requirements needed for manufacturing and assembly.

## Time Spent

| Task | Time |
|---|---|
| Bill of Materials | [INSERT] |
| Labor Cost Calculations | [INSERT] |
| Component Drawings | [INSERT] |
| Assembly Drawing | [INSERT] |
| Documentation | [INSERT] |
| **Total** | **[INSERT]** |

