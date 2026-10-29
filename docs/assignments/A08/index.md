# A08: Gearbox Design

## Objective

The objective of this assignment was to design a functional gearbox that can be assembled and disassembled. This included analyzing the input and output shafts for strength, selecting journal bearings, designing a two-piece housing, and creating a complete SolidWorks assembly.

The project also focused on proper gear alignment, bearing fits, clearances, fastening methods, and engineering drawings following ASME Y14.5 standards.

## Design Requirements

- Gear ratio of 24:9
- Output torque of 1.25 in-lbf
- Output speed of 1100 rpm
- Input shaft diameter of 0.125 in
- Output shaft diameter of 0.250 in
- Shaft lengths of 1.000 in
- Press-fit gears
- Running fits for journal bearings
- Two-piece removable housing
- Proper gear clearances and removable fasteners
- Six individual part drawings and one assembly drawing

## Initial Design Concept

For my gearbox, I chose a simple rectangular housing with a removable top cover. The two housing components are connected using four screws located near the corners.

I selected this design because it is straightforward to model in SolidWorks and allows the gearbox to be assembled and disassembled without damaging the components.

The gearbox contains two spur gears, an input shaft, an output shaft, four sleeve bearings, and a two-piece housing.

## Gear Specifications

| Parameter | Pinion Gear | Output Gear |
|---|---|---|
| McMaster Part Number | 7880K19 | 7880K24 |
| Number of Teeth | 18 | 48 |
| Pitch Diameter | 0.375 in | 1.000 in |
| Shaft Diameter | 0.125 in | 0.250 in |

### Gear Ratio and Center Distance

Gear ratio = 48 / 18 = 2.667

Input speed = 1100 × (48 / 18) = 2933.33 rpm

Input torque = 1.25 × (18 / 48) = 0.46875 in-lbf

Shaft center distance = (0.375 + 1.000) / 2 = 0.6875 in

The larger output gear reduces the rotational speed while increasing the torque.

## Shaft Design

### Shaft Design Overview

Both shafts were analyzed using torsional shear stress equations. I selected AISI 1018 cold-drawn steel as the preliminary material and assumed a factor of safety of 3.

The gear train was assumed to be ideal, and bending moments were neglected according to the assignment instructions.

### Input Shaft

The input shaft has a diameter of 0.125 in and a length of 1.000 in.

- Input speed: 2933.33 rpm
- Input torque: 0.46875 in-lbf
- Calculated shear stress: 1222.3 psi

#### Input Shaft Calculations and FBD

<img width="300" alt="Input shaft calculations and FBD" src="https://github.com/user-attachments/assets/634400ba-56e5-41d9-834e-d28dfe9d2ea6" />

### Output Shaft

The output shaft has a diameter of 0.250 in and a length of 1.000 in.

- Output speed: 1100 rpm
- Output torque: 1.25 in-lbf
- Calculated shear stress: 407.4 psi

#### Output Shaft Calculations and FBD

<img width="352" alt="Output shaft calculations and FBD" src="https://github.com/user-attachments/assets/a6707ae6-d638-4d6c-9d3f-1d72ca23d316" />

### Shaft Results

| Parameter | Input Shaft | Output Shaft |
|---|---|---|
| Diameter | 0.125 in | 0.250 in |
| Length | 1.000 in | 1.000 in |
| Torque | 0.46875 in-lbf | 1.25 in-lbf |
| Shear Stress | 1222.3 psi | 407.4 psi |
| Assumed Allowable Shear Stress | 10,335 psi | 10,335 psi |
| Preliminary Result | Sufficient | Sufficient |

### Shaft Design Conclusion

Based on the simplified torsional loading assumptions, both shafts are sufficient for the required torque. Their calculated shear stresses are below the assumed allowable shear stress.

Therefore, the original shaft diameters were maintained.

These results are based on torsional loading only and do not include additional stresses from bending, stress concentrations, or assembly features.

## Journal Bearing Design

### Bearing Selection

I chose oil-impregnated bronze sleeve bearings because they are commonly used to support rotating shafts and provide a relatively simple bearing design.

The bearings are positioned in the gearbox housing, while the shafts rotate inside them.

Each shaft is supported by two journal bearings, giving the gearbox a total of four bearings.

### Bearing Dimensions

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Shaft Diameter | 0.125 in | 0.250 in |
| Nominal Inside Diameter | 0.125 in | 0.250 in |
| Nominal Outside Diameter | 0.250 in | 0.3125 in |
| Bearing Length | 0.250 in | 0.250 in |
| Intended Material | SAE 841 Bronze | SAE 841 Bronze |
| Shaft Speed | 2933.33 rpm | 1100 rpm |
| Quantity | 2 | 2 |

The bearings were modeled as individual SolidWorks components and inserted into the final assembly.

### Bearing Force Analysis

I calculated the forces acting on the gears to determine the loads transferred to the journal bearings.

For the preliminary analysis, I assumed that each shaft is supported by two bearings sharing the load equally.

#### Bearing Force Calculations and FBD

<img width="348" alt="Bearing force calculations and FBD" src="https://github.com/user-attachments/assets/a6819569-70a0-499f-93f2-406d12aff9d7" />

### Bearing Pressure, Velocity, and PV

The bearing pressure, surface velocity, and PV values were calculated to evaluate the preliminary bearing design.

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Load per Bearing | 1.330 lbf | 1.330 lbf |
| Pressure | 42.56 psi | 21.28 psi |
| Velocity | 96.0 ft/min | 72.0 ft/min |
| PV | 4085.8 psi-ft/min | 1532.2 psi-ft/min |

These values represent the preliminary calculations. Final bearing suitability depends on the actual bearing material ratings, lubrication, operating conditions, and fit clearances.

### Bearing Wall Thickness

The nominal bearing wall thickness was calculated using the inside and outside diameters.

#### Bearing Thickness Calculations and FBD

<img width="351" alt="Bearing wall thickness calculations and FBD" src="https://github.com/user-attachments/assets/6266d9b1-1ca1-452b-ac93-3eaac3280430" />

### Bearing Thickness Results

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Inside Diameter | 0.125 in | 0.250 in |
| Outside Diameter | 0.250 in | 0.3125 in |
| Nominal Wall Thickness | 0.0625 in | 0.03125 in |

These values describe the geometric wall thicknesses. A separate stress-based analysis would be needed to establish a minimum required thickness.

### Bearing Material

SAE 841 oil-impregnated bronze was selected as the intended bearing material.

During SolidWorks modeling, a bronze material from the available material library was used as a substitute where SAE 841 was not available. This material assignment should not be treated as confirmation that the substitute has identical properties to SAE 841.

### McMaster-Carr Bearing References

| Component | Candidate Part Number |
|---|---|
| Input Sleeve Bearing | 1688K321 |
| Output Sleeve Bearing | 6391K126 |

The candidate part numbers and their exact specifications should be verified against the selected bearing dimensions and required running clearances.

[McMaster-Carr Sleeve Bearings](https://www.mcmaster.com/products/journal-bearings/sleeve-bearings-3~/)

## Gearbox Housing Design

### Housing Concept

For the gearbox housing, I designed a rectangular two-piece enclosure consisting of a bottom housing and removable top cover.

The two housing components are connected using four screws near the corners.

The housing supports the bearings and shafts while allowing access to the gears for assembly, inspection, and disassembly.

### Housing Dimensions

| Parameter | Dimension |
|---|---|
| Overall Length | 2.000 in |
| Overall Width | 1.500 in |
| Bottom Housing Height | 0.750 in |
| Top Cover Thickness | 0.125 in |
| Wall Thickness | 0.125 in |
| Bottom Thickness | 0.125 in |
| Shaft Center Distance | 0.6875 in |

The assembled housing height, excluding projecting shafts and screw heads, is approximately 0.875 in.

### Hand-Drawn Housing Sketch

<img width="344" alt="Initial gearbox housing sketch" src="https://github.com/user-attachments/assets/b93883a4-874f-4ccf-9a8b-ddf3db7ee293" />

## SolidWorks Modeling

### Bottom Housing

The bottom housing was created using a rectangular base with a hollow interior.

The modeling process included:

1. Creating a 2.000 in by 1.500 in rectangle.
2. Extruding the rectangle to 0.750 in.
3. Applying a 0.125 in shell thickness.
4. Removing the top face to create the open housing.
5. Adding bearing openings at the required shaft locations.
6. Adding mounting holes for the removable cover.

The shaft center locations were established using the calculated gear center distance of 0.6875 in.

#### Bottom Housing Model

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/0937d5c5-9005-4a63-9a45-ca9d95cc4f48" />

### Top Housing

The top cover was modeled as a separate SolidWorks part.

The cover has an overall size of 2.000 in by 1.500 in with a thickness of 0.125 in.

Bearing openings were positioned to align with the openings in the bottom housing.

Four mounting holes were added near the corners to allow the top cover to be secured with removable screws.

#### Top Housing Model

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/61114c88-b692-48cc-a829-6333ff4e8cc6" />

### Input and Output Shafts

The input and output shafts were modeled as separate cylindrical SolidWorks parts.

| Parameter | Input Shaft | Output Shaft |
|---|---|---|
| Diameter | 0.125 in | 0.250 in |
| Length | 1.000 in | 1.000 in |
| Material | AISI 1018 Steel (intended) | AISI 1018 Steel (intended) |

#### Shaft Models

<p align="center">
  <img width="350" alt="Gearbox Image 1" src="https://github.com/user-attachments/assets/536d187e-7bc5-4f4e-abde-d304efa8e740" />
  <img width="350" alt="Gearbox Image 2" src="https://github.com/user-attachments/assets/9cc1f8af-d6dd-46d9-a13e-3bc02ec23c0c" />
</p>

### Journal Bearing Models

Two different journal bearing parts were created to match the input and output shaft diameters.

Each bearing was modeled as a hollow cylindrical sleeve with the appropriate inside diameter, outside diameter, and length.

Two instances of each bearing were inserted into the gearbox assembly.

#### Bearing Models

<p align="center">
  <img width="350" alt="Gearbox Image 1" src="https://github.com/user-attachments/assets/667a918b-d97d-45c7-8da7-57f50fd95296" />
  <img width="350" alt="Gearbox Image 2" src="https://github.com/user-attachments/assets/acf07b1f-3946-4d3f-a7de-89474aca907d" />
</p>

### Final Gearbox Assembly

The individual components were inserted into a SolidWorks assembly.

The assembly includes:

- One bottom housing
- One top housing
- One 18-tooth pinion gear
- One 48-tooth output gear
- One input shaft
- One output shaft
- Two input journal bearings
- Two output journal bearings
- Four removable screws

The bottom housing was fixed in place, and assembly mates were used to position the remaining components.

Concentric mates aligned the shafts with the bearings and the bearings with the housing openings. Additional mates were used to position the gears, cover, and fasteners.

#### Completed Gearbox Assembly

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/acfc345e-f899-483b-930a-c48f76253735" />

#### Internal Gear and Bearing Assembly

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/1c598601-a67b-4fb7-b5cc-c7eda3d35164" />

## Assembly and Interference Testing

### Gear Alignment

One of the main challenges during assembly was positioning the two spur gears so that they meshed correctly.

During the initial assembly, the gears showed interference when their positions were checked.

I adjusted the gear positions and rotational alignment while maintaining the intended shaft center distance.

This helped me understand how important accurate gear placement is, even when the gear sizes and center distance have already been calculated.

### Bearing Placement

I also had to position the journal bearings correctly in the housing and align them with the shafts.

Concentric and coincident mates were used to establish the bearing and shaft positions.

### Interference Detection

I used the SolidWorks Interference Detection tool to check for overlapping solid geometry.

The initial checks identified interference involving the gears and other assembly components.

After adjusting the component positions and correcting the gear alignment, the final check showed no reported solid interference.

This confirmed that the modeled components were no longer overlapping in the checked assembly position.

However, interference detection at one position does not by itself verify clearance throughout a full gear rotation or confirm the required manufacturing fits.

#### Interference Detection Results


[A08_Output_Bearing.pdf](https://github.com/user-attachments/files/34112733/A08_Output_Bearing.pdf)
[A08_Output_Shaft.pdf](https://github.com/user-attachments/files/34112730/A08_Output_Shaft.pdf)
<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/3d1dcc44-6cfc-48d8-afbd-dc2819b9b77f" />

## Removable Fasteners

The top housing was attached to the bottom housing using four screws inserted near the corners.

The screws were added using the SolidWorks Design Library/Toolbox.

The use of removable fasteners allows the top cover to be removed for access to the internal components.

## Bill of Materials

The final assembly drawing includes the following Bill of Materials.

| Item | Component | Quantity |
|---|---|---|
| 1 | Bottom Housing | 1 |
| 2 | Top Housing | 1 |
| 3 | McMaster 7880K19 Pinion Gear | 1 |
| 4 | McMaster 7880K24 Output Gear | 1 |
| 5 | Input Shaft | 1 |
| 6 | Output Shaft | 1 |
| 7 | Input Journal Bearing | 2 |
| 8 | Output Journal Bearing | 2 |
| 9 | Phillips Machine Screw | 4 |

**Total:** 14 individual components.

## Engineering Drawings

Seven engineering drawings were prepared for the gearbox design: six individual component drawings and one assembly drawing.

The drawings follow a third-angle projection layout and use ASME Y14.5 dimensioning and tolerancing principles.

### Drawing Requirements

- Third-angle projection
- Multiple orthographic views
- Isometric views where helpful
- Section views for internal features
- Complete manufacturing dimensions
- Appropriate tolerance callouts
- Title blocks
- General tolerance block
- At least two different critical-feature tolerancing callouts across the drawing package

### General Tolerances

Unless otherwise specified:

| Dimension | Tolerance |
|---|---|
| X.X | ±0.02 in |
| X.XX | ±0.01 in |
| X.XXX | ±0.005 in |

Specific tolerances for critical mating features should be shown directly on the appropriate part drawings.

### Individual Drawings

| Drawing | Description |
|---|---|
| Input Shaft | Shaft length, diameter, and fit requirements |
| Output Shaft | Shaft length, diameter, and fit requirements |
| Bottom Housing | Overall dimensions, wall thickness, bearing openings, and mounting holes |
| Top Housing | Cover dimensions, bearing openings, and mounting holes |
| Input Bearing | Inside diameter, outside diameter, and length |
| Output Bearing | Inside diameter, outside diameter, and length |
| Gearbox Assembly | Multiview assembly, Section A-A, dimensions, BOM, and balloons |

### Gearbox Assembly Drawing

The final assembly drawing includes top, front, and side views along with an isometric view.

Section A-A was added to show the internal gears, shafts, and bearings.

A Bill of Materials and numbered balloons were also included to identify the individual components.

#### Final Assembly Drawing

<img width="1188" height="842" alt="image" src="https://github.com/user-attachments/assets/08ebbcd0-d589-4182-a1dc-47562a770c85" />

### Individual Part Drawings

<img width="1191" height="846" alt="image" src="https://github.com/user-attachments/assets/0e868b70-39b1-46dd-8605-158832b9c790" />

<img width="1187" height="842" alt="image" src="https://github.com/user-attachments/assets/ad9cba35-149e-418b-8f17-ea2b2884a3de" />

<img width="1187" height="843" alt="image" src="https://github.com/user-attachments/assets/3450dd60-af02-43f6-81e5-416363b30efc" />

<img width="1190" height="837" alt="image" src="https://github.com/user-attachments/assets/b8e56129-0cb6-4bc9-957b-f7e00b0cb06f" />

<img width="1187" height="845" alt="image" src="https://github.com/user-attachments/assets/8e232dac-a045-45ce-b498-78a58d450cb8" />

<img width="1191" height="842" alt="image" src="https://github.com/user-attachments/assets/0b7ff1ac-fb3f-435a-bbda-57cd175a97ca" />

## Final Design Evaluation

The gearbox assembly was completed in SolidWorks using the specified gear ratio, shaft dimensions, and two-piece housing concept.

The assembly contains all major required components, including the gears, shafts, journal bearings, and removable fasteners.

The final interference check showed no reported solid interference at the checked assembly position.

The preliminary shaft stress calculations also indicated that the selected shaft diameters were sufficient for the simplified torsional loading conditions.

Further verification of actual gear running clearance, press fits, journal bearing clearances, material ratings, and manufacturing tolerances is needed to establish full physical functionality.

## Lessons Learned

### Shaft Design

I learned how to calculate torsional shear stress in a solid circular shaft and compare the result to an allowable stress.

I also learned that shaft diameter has a significant effect on torsional stress because the diameter is cubed in the equation.

### Gear Ratios

I learned how the gear ratio affects rotational speed and torque.

The larger output gear reduces rotational speed while increasing torque.

### Journal Bearings

I learned how journal bearing pressure, surface velocity, and PV are related.

I also learned that selecting a bearing requires more than matching its nominal inside diameter to the shaft.

### Housing Design

I learned how to create a two-piece housing using the Shell feature in SolidWorks.

The removable cover made it easier to design an assembly that can be opened without damaging the internal components.

### Assembly Mates

One of the biggest things I learned was how important assembly mates are.

I used concentric and coincident mates to align the shafts, bearings, gears, and housing.

I also learned that adding too many mates or using incorrect mates can cause components to move incorrectly or become overdefined.

### Gear Interference

I initially had problems with the gears interfering and becoming misaligned when rotated.

I had to adjust their positions and check the interference results several times before getting the assembly to the intended configuration.

This helped me understand the importance of checking the complete assembly rather than assuming the parts would fit because their individual dimensions were correct.

### Engineering Drawings

I gained more experience creating multiview drawings, section views, dimensions, title blocks, and Bills of Materials in SolidWorks.

The section view was especially useful because it showed how the internal gears, shafts, and bearings fit inside the housing.


## Time Spent

| Activity | Time |
|---|---|
| Research and Planning | 45 min |
| Shaft Calculations | 45 min |
| Bearing Calculations | 1 hr |
| Housing Design | 45 min |
| SolidWorks Part Modeling | 2 hrs |
| Assembly and Interference Testing | 1 hr 30 min |
| Engineering Drawings | 1 hr 30 min |
| GitHub Documentation | 45 min |
| **Total** | **9 hrs** |

## Final CAD Files

The final CAD package includes:

- Bottom housing SolidWorks part
- Top housing SolidWorks part
- Input shaft SolidWorks part
- Output shaft SolidWorks part
- Input bearing SolidWorks part
- Output bearing SolidWorks part
- Gearbox assembly
- Six individual engineering drawings
- Assembly engineering drawing
- Drawing PDFs

**CAD Downloads:** [A08_Gearbox_Assembly.zip](https://github.com/user-attachments/files/34112835/A08_Gearbox_Assembly.zip)


## References

- Machinery's Handbook, Shafts, pp. 295–297.
- Machinery's Handbook, Gears and Gearing, pp. 2204–2211.
- Machinery's Handbook, Plain Bearing Materials, pp. 2435–2443.
- ASME Y14.5, Dimensioning and Tolerancing.
- D. J. Dunn, *Mechanical Power Transmission Systems: Tutorial Gears*.
- [McMaster-Carr Pinion Gear – 7880K19](https://www.mcmaster.com/7880K19)
- [McMaster-Carr Output Gear – 7880K24](https://www.mcmaster.com/7880K24)
- [McMaster-Carr Sleeve Bearings](https://www.mcmaster.com/products/journal-bearings/sleeve-bearings-3~/)

