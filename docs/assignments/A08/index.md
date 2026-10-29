
# A08: Gearbox Design

## Objective

The objective of this assignment is to design a gearbox that can be assembled and disassembled. This includes analyzing the input and output shafts for strength, selecting journal bearings, and designing a two-piece gearbox housing. SolidWorks will be used to create the parts and final assembly while considering proper clearances, fits, and tolerances.

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
- Proper gear clearances and fasteners

## Initial Design Concept

For my gearbox, I decided to use a simple rectangular housing with a removable top cover. The two housing components will be fastened together using four screws.

I chose this design because it is straightforward to model in SolidWorks and allows the gearbox to be assembled and disassembled without damaging any components.

The gearbox will contain two spur gears, an input shaft, an output shaft, and sleeve bearings to support the shafts.

## Gear Specifications

| Parameter | Pinion Gear | Output Gear |
|---|---|---|
| McMaster Part Number | 7880K19 | 7880K24 |
| Number of Teeth | 18 | 48 |
| Pitch Diameter | 0.375 in | 1.000 in |
| Shaft Diameter | 0.125 in | 0.250 in |

The gear ratio is 2.667, and the calculated shaft center distance is 0.6875 in.

## Shaft Design

### Shaft Design Overview

Both shafts were analyzed using torsional shear stress equations. I selected AISI 1018 cold-drawn steel as the preliminary material and assumed a factor of safety of 3.

The gear train was assumed to be ideal, and bending moments were neglected according to the assignment instructions.

### Input Shaft

The input shaft has a diameter of 0.125 in and a length of 1.000 in.

The calculated input speed is 2933.33 rpm, and the input torque is 0.46875 in-lbf.

#### Input Shaft Calculations and FBD

<img width="300" height="285" alt="image" src="https://github.com/user-attachments/assets/634400ba-56e5-41d9-834e-d28dfe9d2ea6" />

### Output Shaft

The output shaft has a diameter of 0.250 in and a length of 1.000 in.

The output speed is 1100 rpm, and the output torque is 1.25 in-lbf.

#### Output Shaft Calculations and FBD

<img width="352" height="355" alt="image" src="https://github.com/user-attachments/assets/a6707ae6-d638-4d6c-9d3f-1d72ca23d316" />

### Shaft Results

| Parameter | Input Shaft | Output Shaft |
|---|---|---|
| Diameter | 0.125 in | 0.250 in |
| Torque | 0.46875 in-lbf | 1.25 in-lbf |
| Shear Stress | 1222.3 psi | 407.4 psi |
| Allowable Shear Stress | 10,335 psi | 10,335 psi |
| Preliminary Result | Sufficient | Sufficient |

### Shaft Design Conclusion

Based on the simplified torsional loading assumptions, both shafts are sufficient for the required torque. The calculated shear stresses are below the assumed allowable shear stress.

Therefore, the original shaft diameters will be maintained. The material yield strength and any additional loading effects will be verified before finalizing the design.

## Journal Bearing Design

### Bearing Selection

I decided to use oil-impregnated bronze sleeve bearings because they are commonly used to support rotating shafts and provide a simple bearing design.

The bearings will be installed into the gearbox housing, while the shafts rotate inside them.

### Preliminary Bearing Dimensions

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Shaft Diameter | 0.125 in | 0.250 in |
| Bearing Length | 0.250 in | 0.250 in |
| Material | SAE 841 Bronze | SAE 841 Bronze |
| Speed | 2933.33 rpm | 1100 rpm |

### Bearing Force Analysis

I calculated the forces acting on the gears to determine the loads transferred to the journal bearings.

For the preliminary analysis, I assumed that each shaft is supported by two bearings sharing the load equally.

#### Bearing Force Calculations and FBD

<img width="348" height="359" alt="image" src="https://github.com/user-attachments/assets/a6819569-70a0-499f-93f2-406d12aff9d7" />

### Bearing Pressure, Velocity, and PV

The pressure, surface velocity, and PV rating were calculated for both bearings.

### Preliminary Bearing Results

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Load per Bearing | 1.330 lbf | 1.330 lbf |
| Pressure | 42.56 psi | 21.28 psi |
| Velocity | 96.0 ft/min | 72.0 ft/min |
| PV | 4085.8 psi-ft/min | 1532.2 psi-ft/min |

These values will be checked against the allowable bearing material ratings and the final bearing locations.

### Bearing Wall Thickness

The preliminary geometric wall thicknesses were calculated using the selected nominal bearing dimensions.

#### Bearing Thickness Calculations and FBD

<img width="351" height="254" alt="image" src="https://github.com/user-attachments/assets/6266d9b1-1ca1-452b-ac93-3eaac3280430" />

### Preliminary Bearing Thickness Results

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Inside Diameter | 0.125 in | 0.250 in |
| Outside Diameter | 0.250 in | 0.3125 in |
| Nominal Wall Thickness | 0.0625 in | 0.03125 in |

A separate stress-based thickness analysis is required before these dimensions can be finalized.

### McMaster-Carr Bearing Selection

| Component | Candidate Part Number |
|---|---|
| Input Sleeve Bearing | 1688K321 |
| Output Sleeve Bearing | 6391K126 |

The part numbers, dimensions, running clearances, and material ratings will be verified before the final selection.

[McMaster-Carr Sleeve Bearings](https://www.mcmaster.com/products/journal-bearings/sleeve-bearings-3~/)

## Gearbox Housing Design

### Housing Concept

For the gearbox housing, I chose a rectangular two-piece design consisting of a bottom housing and removable top cover.

The two components will be connected using four screws located near the corners.

This design was selected because it is simple to model, allows access to the gears and shafts, and makes assembly and disassembly easier.

### Preliminary Housing Dimensions

| Parameter | Dimension |
|---|---|
| Overall Length | 2.000 in |
| Overall Width | 1.500 in |
| Overall Height | 0.750 in |
| Wall Thickness | 0.125 in |
| Bottom Thickness | 0.125 in |
| Shaft Center Distance | 0.6875 in |

These dimensions may be adjusted to provide sufficient gear clearance, bearing support, and fastening space.

### Hand-Drawn Housing Sketch

<img width="344" height="263" alt="image" src="https://github.com/user-attachments/assets/b93883a4-874f-4ccf-9a8b-ddf3db7ee293" />

## SolidWorks Modeling

### Bottom Housing

I began planning the bottom housing using a rectangular base with a hollow interior.

The preliminary modeling process includes:

1. Create a 2.000 in by 1.500 in rectangle.
2. Extrude the rectangle to 0.750 in.
3. Apply a 0.125 in shell thickness.
4. Remove the top face to create the open housing.
5. Add bearing supports and shaft openings.
6. Add fastening features for the removable cover.

### Bottom Housing Model

![Bottom Housing](images/bottom-housing.png)

### Top Housing

To be completed.

### Final Gearbox Assembly

To be completed.

## Lessons Learned

### Shaft Design

I learned how to calculate torsional shear stress in a solid circular shaft and compare the result to an allowable stress. I also learned that shaft diameter has a significant effect on torsional stress because the diameter is cubed in the equation.

### Gear Ratios

I learned how the gear ratio affects rotational speed and torque. The larger output gear reduces the rotational speed while increasing the torque.

### Journal Bearings

I learned how journal bearing pressure, surface velocity, and PV are related. I also learned that selecting a bearing requires more than matching its nominal inside diameter to the shaft.

### Housing Design

During the initial design process, I chose a rectangular housing because it would be easier to model and assemble. I also learned that the center distance between the gears is important for proper meshing.

## Time Spent

| Activity | Time |
|---|---|
| Research and Planning | To be recorded |
| Shaft Calculations | To be recorded |
| Bearing Calculations | To be recorded |
| Housing Design | To be recorded |
| SolidWorks Modeling | To be recorded |
| Drawings and Documentation | To be recorded |
| **Total** | **To be calculated** |

## Engineering Drawings

The following drawings will be included once the CAD models are completed:

1. Input shaft
2. Output shaft
3. Bottom housing
4. Top housing
5. Input journal bearing
6. Output journal bearing
7. Gearbox assembly

All drawings will use third-angle projection and appropriate ASME Y14.5 dimensioning and tolerancing.

General tolerance block:

| Dimension | Tolerance |
|---|---|
| X.X | ±0.02 in |
| X.XX | ±0.01 in |
| X.XXX | ±0.005 in |

Critical mating features will receive specific fit tolerances.

## Final CAD Files

Download CAD Files: Link to be added.

## References

- Machinery's Handbook, Shafts, pp. 295–297.
- Machinery's Handbook, Gears and Gearing, pp. 2204–2211.
- Machinery's Handbook, Plain Bearing Materials, pp. 2435–2443.
- D. J. Dunn, Mechanical Power Transmission Systems: Tutorial Gears.
- [McMaster-Carr Pinion Gear](https://www.mcmaster.com/7880K19)
- [McMaster-Carr Output Gear](https://www.mcmaster.com/7880K24)
- [McMaster-Carr Sleeve Bearings](https://www.mcmaster.com/products/journal-bearings/sleeve-bearings-3~/)



