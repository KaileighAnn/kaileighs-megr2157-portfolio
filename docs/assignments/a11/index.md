
# A11 – Motor Selection and Tensile Tester Design

## Team Members

- **Kelsey Skipper** – Engineering calculations, motor selection, and component analysis
- **Gracie Steelmon** – Motor mount CAD, assembly updates, and FEA
- **Kaileigh Hill** – Bill of materials, labor costs, documentation, and MEGR 2157 engineering drawings

## Project Objective

The objective of A11 was to continue the design of the bench-top tensile tester developed in A10. The system uses two lead screws to move a crosshead and is designed for a maximum tensile load of **2,000 N**. This phase focused on motor selection, supporting component calculations, CAD updates, structural analysis, cost estimates, and engineering drawings.

### Design Requirements

| Parameter | Value |
|---|---:|
| Maximum tensile load | 2,000 N |
| Load per lead screw | 1,000 N |
| Required factor of safety | 4 |
| Crosshead speed | 1–50 mm/min |
| Lead screw diameter | 3/8 in |
| Lead screw length used in A11 calculations | 24 in |
| Lead screw thread | 3/8-12 ACME |
| Calculated operating torque | 4.759 N·m |
| Design torque | 19.036 N·m |
| Required rotational speed | 0.473–23.62 RPM |

*The A10 documentation listed 3-ft lead screws, while A11 calculations use 24 in. The final purchased length should be confirmed against the CAD model.*

---

## 1. Engineering Calculations and Motor Selection

### 1.1 Motor Selection

Two [McMaster-Carr DC gearmotors (6470K84)](https://www.mcmaster.com/6470K84/) were selected, one for each lead screw. Each motor has a listed rated torque of **24.857 N·m** and rated speed of **31 RPM**. The rated torque exceeds the calculated design torque of **19.036 N·m**. Operation throughout the required low-speed range still needs verification using the motor's torque-speed characteristics.

<img src="https://github.com/user-attachments/assets/9a6996eb-44a8-4d83-a464-82720e6b1d81" width="750" alt="Motor selection calculations">

**Figure 1:** Motor selection and torque calculations.

<img src="https://github.com/user-attachments/assets/bc217370-819a-4948-9e19-d67b5a2ef96b" width="500" alt="Selected motor specifications">

**Figure 2:** Selected DC gearmotor specifications.

### 1.2 Motor Mount Analysis

**6061-T6 aluminum** was selected for the motor mounting brackets because of its strength, low weight, and machinability. The mounting bolt reactions and minimum bracket thickness were evaluated using allowable bearing stress.

<img src="https://github.com/user-attachments/assets/e4f8e94c-af0f-4362-a341-dde0a9757f14" width="750" alt="Motor mount bearing stress calculations">

**Figure 3:** Motor mounting bracket calculations.

### 1.3 Coupler Analysis

A proposed motor-to-lead-screw coupler was evaluated using torsional shear stress equations to estimate its minimum outside diameter and wall thickness. The proposed material was **6061-T6 aluminum**, and the motor-side opening must accommodate the selected motor's **15.875 mm output shaft**.

<img src="https://github.com/user-attachments/assets/32f3199c-6238-4d86-8980-e942582fc552" width="750" alt="Coupler torsional calculations">

**Figure 4:** Coupler torsional stress calculations.

*The coupler was analyzed but was not included in the submitted CAD assembly.*

### 1.4 Frame Connector Analysis

Vertical and transverse reaction forces were calculated for the frame connections based on the applied loads and motor reaction moments. These calculations were used to evaluate connector stresses and required thickness.

<img src="https://github.com/user-attachments/assets/6c29c214-e570-498b-801e-90fa1341909e" width="750" alt="Frame connector calculations">

**Figure 5:** Frame connection calculations.

*Separate corner brackets were not included in the submitted CAD assembly.*

### 1.5 Horizontal Frame Analysis

The horizontal frame members use **heavy 40 Series aluminum T-slot extrusion**. The loading conditions established for FEA were two **1,000 N** axial loads and two motor reaction moments of approximately **25 N·m**.

<img src="https://github.com/user-attachments/assets/257fe632-75c8-437f-8d8d-da1577e5486e" width="750" alt="Horizontal frame loading calculations">

**Figure 6:** Horizontal frame loading calculations.

### 1.6 Vertical Frame Analysis

The vertical frame members were evaluated under axial compression and transverse loading from the motor reaction moments, with a target factor of safety of **4**.

<img src="https://github.com/user-attachments/assets/d7c3873f-7bf6-4ed2-9c3e-936bf32fc5ed" width="750" alt="Vertical frame calculations">

**Figure 7:** Vertical frame calculations.

### 1.7 Floating Bearing Fit

An **RC3 running fit** was selected for the proposed floating bearing interface. The analysis considered shaft and hole tolerances, clearance limits, and mounting bolt clearance requirements.

<img src="https://github.com/user-attachments/assets/bb661d98-5aed-4e39-83a1-99564ad583f8" width="750" alt="RC3 fit calculations">

**Figure 8:** Floating bearing RC3 fit calculations.

<img src="https://github.com/user-attachments/assets/ef7e0db4-5df1-47b1-be97-cb71e951ad53" width="650" alt="Floating bearing mounting calculations">

**Figure 9:** Additional bearing mount and clearance calculations.

*The floating bearing mount was analyzed but was not identified as a modeled component in the submitted assembly.*

### 1.8 Component and Material Selections

| Component | Selected material or specification |
|---|---|
| DC gearmotors | McMaster-Carr 6470K84 |
| Lead screws | 1080 carbon steel, 3/8-12 ACME |
| Lead screw nuts | SAE 932 bearing bronze |
| Motor mounting brackets | 6061-T6 aluminum |
| Proposed couplers | 6061-T6 aluminum |
| Proposed frame connectors | 6061-T6 aluminum |
| Horizontal and vertical frame | Heavy 40 Series aluminum T-slot extrusion |
| Proposed floating bearing mounts | 6061-T6 aluminum |
| Fasteners | Steel / selected stainless steel hardware |

These selections were based on strength, machinability, availability, and compatibility with the tensile tester. Final verification depends on the FEA results and the actual component specifications.

---

## 2. SolidWorks CAD and Finite Element Analysis

### 2.1 Motor Mount Bracket and Assembly

Using the motor mount calculations, the mounting bracket was modeled in SolidWorks and added to the existing A10 tensile tester assembly.

<img src="https://github.com/user-attachments/assets/a1085504-8fa4-4a4e-b3ba-a5e19ddcca66" width="750" alt="Motor mounting bracket CAD">

**Figure 10:** Motor mounting bracket CAD model.

### 2.2 Fastener Selection

The bracket hole diameter was **6.6 mm**. The team selected **M4 × 0.7 mm**, **70 mm** long 18-8 stainless steel screws and matching nuts. The selected length was based on the combined component thickness, with additional thread length for nut engagement.

<img src="https://github.com/user-attachments/assets/1571c766-708f-41bd-84e3-2383c41fd2ae" width="700" alt="Selected mounting screw">

**Figure 11:** Selected mounting screw.

<img src="https://github.com/user-attachments/assets/3fbd0ece-8c9d-4f42-b50b-8665ed00ff3d" width="700" alt="Selected mounting nut">

**Figure 12:** Selected mounting nut.

<img src="https://github.com/user-attachments/assets/755ec001-5631-436f-96a5-6d5318dd7a6d" width="700" alt="Mounting hardware dimensions">

**Figure 13:** Mounting hardware specifications.

*The 6.6 mm holes are considerably larger than the nominal 4 mm screw diameter. The fit and bolt loading should be checked before manufacturing.*

### 2.3 FEA Setup

A SolidWorks Simulation study was created with the bottom of the bracket fixed. Two **1,000 N downward loads** were applied at the lead screw locations, along with a **24.857 N·m** motor reaction torque at the mounting regions.

<img src="https://github.com/user-attachments/assets/1f53a527-4558-45c3-95c4-e20c1afe05c6" width="750" alt="FEA fixed geometry">

**Figure 14:** Fixed geometry for the FEA study.

<img src="https://github.com/user-attachments/assets/335c16fd-3642-4dca-b334-5ea432f82544" width="750" alt="FEA applied forces">

**Figure 15:** Applied loads and motor torque.

<img src="https://github.com/user-attachments/assets/46b9834c-2a4f-4a5f-bfaf-96e327b5e141" width="750" alt="FEA setup additional view">

**Figure 16:** Additional FEA setup view.

### 2.4 Mesh

The initial medium mesh did not generate correctly, and a coarser mesh also caused problems. After retrying the medium mesh, the simulation generated successfully.

### 2.5 FEA Results

The study was reviewed using von Mises stress, factor of safety, and strain plots.

<img src="https://github.com/user-attachments/assets/2d898f73-c823-4d27-ada1-fb55e13b7eb8" width="750" alt="Von Mises stress results">

**Figure 17:** Von Mises stress results.

<img src="https://github.com/user-attachments/assets/3d213265-15a0-4a0c-88ba-adc5180b6d2d" width="750" alt="Factor of safety results">

**Figure 18:** Factor of safety results.

<img src="https://github.com/user-attachments/assets/bbbaa978-45cc-4060-aa4f-eca9d73241d7" width="750" alt="Strain results">

**Figure 19:** Strain results.

### 2.6 Evaluation

The simulation suggested that the applied motor torque had a greater effect on the bracket than the axial loads. A possible improvement would be to select a stronger material or revise the bracket geometry. The final design should be checked against the required factor of safety before manufacturing.

---

## 3. Bill of Materials and Engineering Labor

### 3.1 Bill of Materials

The table combines the previously selected A10 components with the A11 motor and hardware selections. Prices marked with an asterisk are estimates.

| Component | Qty. | Unit Cost | Total | Supplier |
|---|---:|---:|---:|---|
| 3/8"-12 ACME Lead Screw | 2 | $35.32 | $70.64 | [McMaster-Carr](https://www.mcmaster.com/99030A993/) |
| Bronze Flange Nut | 2 | $111.78 | $223.56 | [McMaster-Carr](https://www.mcmaster.com/95120A592/) |
| T-Slot Framing | 1 | $245.87 | $245.87 | [Grainger](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48) |
| DC Gearmotor | 2 | $500.00* | $1,000.00 | [McMaster-Carr](https://www.mcmaster.com/6470K84/) |
| Thrust Bearing | 2 | $25.00* | $50.00 | [McMaster-Carr](https://www.mcmaster.com/thrust-bearings/) |
| Bronze Bushing | 2 | $5.00* | $10.00 | [McMaster-Carr](https://www.mcmaster.com/bushings/) |
| M4 × 0.7 mm, 70 mm Screws (pack of 10) | 1 pack | $12.88 | $12.88 | [McMaster-Carr](https://www.mcmaster.com/92010A819/) |
| M4 × 0.7 mm Hex Nuts (pack of 4,000) | 1 pack | $85.12 | $85.12 | McMaster-Carr |
| Assorted Mounting Hardware | 1 set | $40.00* | $40.00 | [McMaster-Carr](https://www.mcmaster.com/) |
| **Priced Material Subtotal** | | | **$1,738.07** | |

*This is a preliminary cost estimate, not a complete as-built BOM. Purchased motors, thrust bearings, bushings, and proposed components are not all shown in the current CAD assembly. Custom-fabricated parts and any additional frame connections have not been priced. The $40 hardware allowance should be checked to avoid double counting the listed screws and nuts.*

### 3.2 Engineering Labor Costs

Engineering labor was calculated at the required rate of **$35 per hour**, including the work completed in both A10 and A11.

| Team Member | A10 Hours | A11 Hours | Total Hours | Labor Cost |
|---|---:|---:|---:|---:|
| Kaileigh Hill | 4 | 4 | 8 | $280.00 |
| Kelsey Skipper | 3 | 5 | 8 | $280.00 |
| Gracie Steelmon | 5 | 5 | 10 | $350.00 |
| **Total** | **12** | **14** | **26** | **$910.00** |

**Labor Cost = Total Hours × $35/hr**

### 3.3 Total Engineering Cost

| Category | Cost |
|---|---:|
| Priced Materials | $1,738.07 |
| A10 Engineering Labor (12 hours) | $420.00 |
| A11 Engineering Labor (14 hours) | $490.00 |
| **Current Project Total** | **$2,648.07** |

*The current project total includes the materials priced so far and all reported engineering labor. It excludes unpriced custom components and additional fabrication costs.*

---

## 4. MEGR 2157 – Engineering Drawing Package

### 4.1 Objective

The objective of this portion was to prepare engineering drawings of the components modeled for the tensile tester and document the overall assembly. The drawings communicate dimensions, tolerances, materials, and assembly information.

### 4.2 Drawing Standards

The drawings use **third-angle projection**, **ASME Y14.5** dimensioning and tolerancing conventions, and the following general inch tolerances:

| Dimension Precision | General Tolerance |
|---|---|
| X.X | ±0.02 in |
| X.XX | ±0.01 in |
| X.XXX | ±0.005 in |

Drawing sheets include title blocks with the part or assembly name, scale, and drawing information.

### 4.3 Crosshead Drawing (A10)

The previously completed crosshead drawing shows the part dimensions and lead screw mounting locations.

<img src="https://github.com/user-attachments/assets/75371664-f118-46c5-852b-8c5e30228bd8" width="750" alt="Crosshead engineering drawing">

**Figure 20:** Crosshead engineering drawing from A10.

### 4.4 Motor Mount Bracket Drawing

A detailed drawing was prepared for the motor mounting bracket, including orthographic and isometric views, mounting holes, and dimensions.

<img src="https://github.com/user-attachments/assets/974c1fb8-5c24-4379-bd07-07a4157b4e12" width="750" alt="Motor mounting bracket engineering drawing">

**Figure 21:** Motor mounting bracket engineering drawing.

### 4.5 Final Assembly Drawing

The final SolidWorks assembly drawing shows the modeled tensile tester frame, crosshead, lead screws, bronze flange nuts, mounting brackets, and fasteners. The drawing includes an isometric view, a Bill of Materials, and numbered balloons identifying the components.

<img width="1612" height="873" alt="Assem2" src="https://github.com/user-attachments/assets/19210085-4985-4894-a918-28cd5d74febf" />

**Figure 22:** Final tensile tester assembly drawing with BOM and item balloons.

*The drawing documents the current CAD assembly; components selected or analyzed but not modeled are not shown as installed.*

### 4.6 CAD and Drawing Files

[Download SolidWorks CAD Assembly (Assem2.zip)](https://github.com/user-attachments/files/35060613/Assem2.zip)

---

## 5. Lessons Learned

### Kelsey Skipper – Engineering Calculations

Through this assignment, I learned how motor torque affects the design of mechanical components and supporting structures. I gained a better understanding of bearing tolerances, torsional loading, and how hand calculations support FEA. I also learned the importance of verifying purchased component specifications before finalizing a design.

### Gracie Steelmon – CAD and FEA

Through this assignment, I improved my SolidWorks CAD skills by designing the motor mounting brackets and working with the tensile tester assembly. I became more comfortable modeling parts and understanding how they fit together. I also gained more experience setting up and troubleshooting FEA simulations.

### Kaileigh Hill – BOM and MEGR 2157 Drawings

Through this assignment, I learned how to organize a Bill of Materials and calculate engineering labor costs. For the MEGR 2157 portion, I gained experience creating engineering drawings in SolidWorks, adding dimensions and tolerances, editing title blocks, and creating an assembly drawing with a BOM and numbered balloons.

---

## 6. Project Time

### A10 and A11 Team Hours

| Team Member | A10 Hours | A11 Hours | Total Hours |
|---|---:|---:|---:|
| Kaileigh Hill | 4 | 4 | 8 |
| Kelsey Skipper | 3 | 5 | 8 |
| Gracie Steelmon | 5 | 5 | 10 |
| **Total** | **12** | **14** | **26** |

## 7. References and Resources

1. [McMaster-Carr – ACME Lead Screw](https://www.mcmaster.com/99030A993/)
2. [McMaster-Carr – Bronze Flange Nut](https://www.mcmaster.com/95120A592/)
3. [McMaster-Carr – DC Gearmotor](https://www.mcmaster.com/6470K84/)
4. [McMaster-Carr – M4 Mounting Screws](https://www.mcmaster.com/92010A819/)
5. [Grainger – T-Slot Framing](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48)
6. SolidWorks and SolidWorks Simulation
7. *Machinery's Handbook*, 31st Edition
8. MEGR 2156 and MEGR 2157 course materials
