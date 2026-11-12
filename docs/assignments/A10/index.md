# A10 – Lead Screw Translating System

## Parametric Modeling and CAD Assembly – Kaileigh Hill

### Objective

The objective of my portion of this project was to create a 3D CAD model of the tensile tester using SolidWorks. I modeled the crosshead and assembled the selected lead screws, bronze flange nuts, and framing components. The goal was to create an assembly that represents how the mechanical components fit together using the dimensions established through our team's calculations.

### 1. Crosshead Modeling

I began by creating the crosshead in SolidWorks using the dimensions determined through our team's calculations. I sketched a rectangular profile and used the Extruded Boss/Base feature to create the initial solid.

Next, I created two circular openings for the lead screws and bronze flange nuts. The openings were positioned symmetrically near each end of the crosshead and created using the Extruded Cut feature.

**Crosshead Dimensions:**

| Feature | Dimension |
|---|---|
| Length | 12.00 in |
| Width | 3.00 in |
| Height | 3.684 in |
| Lead Screw Opening Diameter | 0.510 in |
| Lead Screw Center Spacing | 10.00 in |
| Material | A36 Low Carbon Steel |

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/dde21ab3-a162-4c19-b113-25595c0aabb6" />

*Figure 1: Initial SolidWorks crosshead model before adding the lead screw openings.*

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/c9d4eb3e-d79a-4626-9064-69ef4d9a6c7d" />

*Figure 2: Completed crosshead model showing the two lead screw openings.*

### 2. Downloading CAD Components

After modeling the crosshead, I downloaded the manufacturer CAD files for the lead screws and bronze flange nuts from McMaster-Carr. Using existing CAD files allowed me to incorporate accurate component geometry without modeling commercially available parts from scratch.

The components included:

- Two 3/8"-12 Acme lead screws made from 1018 carbon steel.
- Two 3/8"-12 Acme flange nuts made from 932 bearing bronze.
- T-slot framing components obtained from Grainger.

**Component Links:**

- [Acme Lead Screw – McMaster-Carr](https://www.mcmaster.com/99030A993/)
- [Bronze Flange Nut – McMaster-Carr](https://www.mcmaster.com/95120A592/)
- [T-Slot Framing – Grainger](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48)

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/67b3ee42-274f-4259-9dd5-ecd0a2453d9f" />

*Figure 3: Manufacturer CAD model of the bronze Acme flange nut.*

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/62e8d474-b98e-4cfc-9dce-502b1d3796c5" />

*Figure 4: Manufacturer CAD model of the 3/8"-12 Acme lead screw.*

### 3. SolidWorks Assembly

After obtaining the necessary CAD components, I created a new assembly in SolidWorks.

I inserted the crosshead first and used it as the reference component for the assembly. I then inserted two bronze flange nuts and aligned them with the crosshead openings using Concentric Mates.

Coincident Mates were used to position the flange surfaces against the crosshead. The nuts were oriented with the flanges underneath the crosshead to establish a direct load path for the proposed downward tensile loading arrangement.

Next, I inserted two Acme lead screws and aligned them with their corresponding flange nuts.

Finally, I incorporated the framing components into the assembly to represent the overall tensile tester structure.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/3d28f4ba-af76-4e79-ae5c-d5eaef791a7f" />

*Figure 5: Crosshead assembly showing both bronze flange nuts positioned underneath the crosshead.*

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/d78998ab-44d5-4194-861c-32d321561d8b" />

*Figure 6: SolidWorks assembly showing the lead screws aligned with the crosshead and bronze flange nuts.*

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/f0d4743e-ddaa-48bc-950b-b4cef81cd20d" />

*Figure 7: Overall SolidWorks CAD assembly of the tensile tester.*

### 7. CAD Files

The SolidWorks CAD files for this project are available in the downloadable ZIP folder below.

**[Download SolidWorks CAD Files](https://github.com/user-attachments/files/34669260/Assem2.zip)**

The folder includes the crosshead, lead screws, bronze flange nuts, framing components, and overall assembly.


aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa


# A10 – Lead Screw Translating System Design

## Group Members

- **Gracie Steelmon** – Lead Screw and Crosshead Calculations
- **Kaileigh Hill** – Parametric Modeling and CAD Assembly
- **Kelsey Skipper** – MEGR 2157 Analysis and Documentation

---

## Project Objective

The objective of this project was to conceptually design a mechanically driven tensile testing system capable of applying a controlled axial tensile load of up to **2 kN** to a material specimen.

A tensile tester is used to evaluate the mechanical properties of materials by applying a controlled pulling force and measuring the resulting deformation. This allows engineers to determine material properties such as yield strength, ultimate tensile strength, and elongation at failure.

Our proposed design uses two Acme lead screws to translate a crosshead vertically, allowing a tensile force to be applied to the specimen. The system was designed to emphasize structural strength, controlled movement, proper component alignment, and minimal crosshead deflection.

### Design Requirements

| Design Parameter | Requirement |
|---|---|
| Maximum Tensile Load | 2 kN |
| Crosshead Speed | 1–50 mm/min |
| Minimum Lead Screw Length | 18 in |
| Number of Lead Screws | 2 |
| Required Safety Factor | 4 |
| Maximum Crosshead Deflection | 0.1 mm |
| Operating System | Fully Mechanical |
| Configuration | Bench-Top Tensile Tester |

### Project Scope

The project involved:

1. Determining the minimum lead screw diameter using axial stress analysis.
2. Calculating the required lead screw rotational speed range.
3. Determining the torque required to produce the specified tensile load.
4. Selecting appropriate Acme lead screws and bronze flange nuts.
5. Analyzing crosshead strength and deflection.
6. Developing a preliminary multiview crosshead sketch.
7. Tabulating the costs of commercially available components.
8. Creating a SolidWorks model and assembly of the proposed tensile tester.
9. Performing additional FEA and engineering drawing work for MEGR 2157.

The overall goal was to develop a mechanically feasible tensile tester design that could provide consistent loading while maintaining structural integrity and alignment.

---

<div style="background-color: #DDF3E4; color: #243B2B; padding: 20px; border-radius: 10px;" markdown="block">

## 1. Lead Screw Diameter Analysis – Gracie Steelmon

### 1.1 Minimum Lead Screw Diameter

The minimum diameter of the lead screws was determined using axial stress analysis.

Because the tensile tester uses two identical lead screws, the applied 2 kN tensile load was assumed to be distributed equally between them.

The force supported by each lead screw was therefore:

**Force per Lead Screw = 1,000 N**

A safety factor of 4 was applied when determining the minimum acceptable screw diameter.

The analysis included identifying the known and unknown variables, developing a free-body diagram, solving the governing equations symbolically, and calculating the required diameter numerically.

![Lead Screw Diameter Calculations](leadscrewdiameter.jpg)

*Figure 1: Axial stress analysis used to determine the minimum lead screw diameter.*

---

## 2. Lead Screw Rotational Speed – Gracie Steelmon

### 2.1 Rotational Speed Range

The required rotational speed range was determined using the specified crosshead translation speed of 1–50 mm/min.

The relationship between linear translation and rotational speed depends on the lead of the selected screw.

For a lead screw, the linear translation per revolution is equal to the screw lead.

The governing relationship is:

**Linear Speed = Rotational Speed × Screw Lead**

Rearranging:

**Rotational Speed = Linear Speed / Screw Lead**

The calculations were used to determine the rotational speeds necessary to achieve the required crosshead movement.

![Rotational Speed Calculations](rangerotationalspeed.jpg)

*Figure 2: Calculations determining the required lead screw rotational speed range.*

---

## 3. Lead Screw Torque and Selection – Gracie Steelmon

### 3.1 Maximum Torque Analysis

The maximum torque required to produce the specified 2 kN tensile load was determined using lead screw mechanics.

This analysis considered the relationship between rotational input torque and the resulting axial force.

The torque requirement is influenced by the applied load, screw geometry, thread friction, and lead angle.

The calculations were used to evaluate the torque required to operate the proposed system.

![Lead Screw Selection Calculations](selectingleadscrew.jpg)

*Figure 3: Torque analysis used to evaluate and select the lead screws.*

### 3.2 Final Lead Screw Selection

The selected component was a **right-hand, 3/8"-12 Acme lead screw**, specified as 1018 carbon steel in the original selection notes.

A 3-foot length was selected because the alternative 18-inch length was insufficient for the proposed design.

The longer screw provides additional material for cutting to the required assembly length.

**Selected Component:**

| Feature | Specification |
|---|---|
| Thread Type | Acme |
| Thread Size | 3/8"-12 |
| Thread Direction | Right-Hand |
| Material | Carbon Steel – Grade to Verify |
| Purchased Length | 3 ft |
| Quantity | 2 |

[McMaster-Carr Lead Screw](https://www.mcmaster.com/99030A993/)

**Material Verification:** The original selection notes specify 1018 carbon steel, while the initial cost table lists 1080 carbon steel. The material grade should be confirmed using the selected supplier part number.

---

## 4. Bronze Nut and Flange Selection – Gracie Steelmon

### 4.1 Internal Thread Analysis

The bronze flange nuts were selected to support the axial loading transmitted through the lead screws.

Thread bending stress analysis was performed to evaluate whether the internal threads could withstand the applied load while satisfying the required safety factor.

The analysis included identifying the known and unknown variables, developing a free-body diagram, solving the governing equations symbolically, and calculating the thread bending stress numerically.

![Bronze Nut Selection](selectingnut.jpg)

*Figure 4: Internal thread analysis used to evaluate the bronze flange nut.*

### 4.2 Selected Component

| Feature | Specification |
|---|---|
| Component | Acme Bronze Flange Nut |
| Thread Size | 3/8"-12 |
| Thread Direction | Right-Hand |
| Material | Bearing Bronze |
| Quantity | 2 |

[McMaster-Carr Bronze Flange Nut](https://www.mcmaster.com/95120A592/)

---

## 5. Crosshead Stress and Strength Analysis – Gracie Steelmon

### 5.1 Beam Strength Analysis

The crosshead was designed to transfer the tensile testing load between the two lead screws while maintaining structural integrity.

Simple beam stress and strength calculations were used to evaluate the required crosshead dimensions and material.

The analysis considered the applied loading, support locations, bending stress, and required safety factor.

The crosshead was treated as a structural member subjected to loading from the tensile specimen and supported at the lead screw locations.

![Crosshead Strength Analysis](designcrosshead.jpg)

*Figure 5: Beam stress and strength analysis for the tensile tester crosshead.*

---

## 6. Crosshead Beam Deflection Analysis – Gracie Steelmon

### 6.1 Deflection Requirements

The crosshead was evaluated for vertical deflection under the applied 2 kN tensile load.

The maximum allowable deflection was specified as **0.1 mm**.

Beam deflection equations were used to evaluate the relationship between material stiffness, crosshead geometry, and applied loading.

The analysis helped establish the crosshead dimensions necessary to limit bending during tensile testing.

![Beam Deflection Analysis](beamdeflectionanalysis.jpg)

*Figure 6: Beam deflection calculations used to evaluate crosshead stiffness.*

---

## 7. Crosshead Multiview Sketch – Gracie Steelmon

### 7.1 Preliminary Crosshead Design

A preliminary multiview sketch was created to communicate the proposed crosshead geometry.

The sketch includes the overall dimensions, lead screw locations, and mounting features required for the bronze flange nuts.

The purpose of the sketch was to establish the initial geometry before creating the SolidWorks model.

![Crosshead Multiview Sketch](multiviewsketch.jpg)

*Figure 7: Preliminary multiview engineering sketch of the crosshead.*

</div>

---

## 8. Material Cost Analysis

The cost of the commercially available mechanical components was estimated using supplier pricing.

The following table includes the selected components, quantities, individual prices, and total estimated costs.

| Item | Quantity | Component | Cost per Item | Total Cost | Purchase Link |
|---|---|---|---|---|---|
| 1 | 2 | Carbon Steel Acme Lead Screw, RH, 3/8"-12, 3 ft | $35.32 | $70.64 | [McMaster-Carr](https://www.mcmaster.com/99030A993/) |
| 2 | 2 | Acme Bronze Flange Nut, RH, 3/8"-12 | $111.78 | $223.56 | [McMaster-Carr](https://www.mcmaster.com/95120A592/) |
| 3 | 1 | T-Slot Framing System | $245.87 | $245.87 | [Grainger](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48) |
| | | | **Total Estimated Cost** | **$540.07** | |

The total estimated purchased component cost was **$540.07**, excluding custom-fabricated parts, machining, and other unlisted hardware.

---

<div style="background-color: #FCE3E3; color: #4A2424; padding: 20px; border-radius: 10px;" markdown="block">

## 9. Parametric Modeling and CAD Assembly – Kaileigh Hill

### Objective

The objective of my portion of this project was to create a 3D CAD model of the tensile tester using SolidWorks.

I modeled the crosshead and assembled the selected lead screws, bronze flange nuts, and framing components.

The goal was to create an assembly that represents how the mechanical components fit together using the dimensions established through our team's calculations.

### 9.1 Crosshead Modeling

I began by creating the crosshead in SolidWorks using the dimensions determined through our team's calculations.

I sketched a rectangular profile and used the Extruded Boss/Base feature to create the initial solid.

Next, I created two circular openings for the lead screws and bronze flange nuts.

The openings were positioned symmetrically near each end of the crosshead and created using the Extruded Cut feature.

**Crosshead Dimensions:**

| Feature | Dimension |
|---|---|
| Length | 12.00 in |
| Width | 3.00 in |
| Height | 3.684 in |
| Lead Screw Opening Diameter | 0.510 in |
| Lead Screw Center Spacing | 10.00 in |
| Material | A36 Low Carbon Steel |

<img width="960" alt="Initial Crosshead Model" src="https://github.com/user-attachments/assets/dde21ab3-a162-4c19-b113-25595c0aabb6" />

*Figure 8: Initial SolidWorks crosshead model before adding the lead screw openings.*

<img width="960" alt="Completed Crosshead Model" src="https://github.com/user-attachments/assets/c9d4eb3e-d79a-4626-9064-69ef4d9a6c7d" />

*Figure 9: Completed crosshead model showing the two lead screw openings.*

### 9.2 Downloading CAD Components

After modeling the crosshead, I downloaded the manufacturer CAD files for the lead screws and bronze flange nuts from McMaster-Carr.

Using existing CAD files allowed me to incorporate accurate component geometry without modeling commercially available parts from scratch.

The components included:

- Two 3/8"-12 Acme lead screws made from 1018 carbon steel, as specified in the original selection notes.
- Two 3/8"-12 Acme flange nuts made from 932 bearing bronze.
- T-slot framing components obtained from Grainger.

**Component Links:**

- [Acme Lead Screw – McMaster-Carr](https://www.mcmaster.com/99030A993/)
- [Bronze Flange Nut – McMaster-Carr](https://www.mcmaster.com/95120A592/)
- [T-Slot Framing – Grainger](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48)

<img width="960" alt="Bronze Flange Nut" src="https://github.com/user-attachments/assets/67b3ee42-274f-4259-9dd5-ecd0a2453d9f" />

*Figure 10: Manufacturer CAD model of the bronze Acme flange nut.*

<img width="960" alt="Acme Lead Screw" src="https://github.com/user-attachments/assets/62e8d474-b98e-4cfc-9dce-502b1d3796c5" />

*Figure 11: Manufacturer CAD model of the 3/8"-12 Acme lead screw.*

### 9.3 SolidWorks Assembly

After obtaining the necessary CAD components, I created a new assembly in SolidWorks.

I inserted the crosshead first and used it as the reference component for the assembly.

I then inserted two bronze flange nuts and aligned them with the crosshead openings using Concentric Mates.

Coincident Mates were used to position the flange surfaces against the crosshead.

The nuts were oriented with the flanges underneath the crosshead to establish a direct load path for the proposed downward tensile loading arrangement.

Next, I inserted two Acme lead screws and aligned them with their corresponding flange nuts.

Finally, I incorporated the framing components into the assembly to represent the overall tensile tester structure.

<img width="960" alt="Crosshead and Flange Nuts" src="https://github.com/user-attachments/assets/3d28f4ba-af76-4e79-ae5c-d5eaef791a7f" />

*Figure 12: Crosshead assembly showing both bronze flange nuts positioned underneath the crosshead.*

<img width="960" alt="Lead Screw Assembly" src="https://github.com/user-attachments/assets/d78998ab-44d5-4194-861c-32d321561d8b" />

*Figure 13: SolidWorks assembly showing the lead screws aligned with the crosshead and bronze flange nuts.*

<img width="960" alt="Overall Tensile Tester Assembly" src="https://github.com/user-attachments/assets/f0d4743e-ddaa-48bc-950b-b4cef81cd20d" />

*Figure 14: Overall SolidWorks CAD assembly of the tensile tester.*

### 9.4 CAD Files

The SolidWorks CAD files for this project are available in the downloadable ZIP folder below.

**[Download SolidWorks CAD Files](https://github.com/user-attachments/files/34669260/Assem2.zip)**

The folder includes the crosshead, lead screws, bronze flange nuts, framing components, and overall assembly.

</div>

---

<div style="background-color: #E8F1FA; color: #243B53; padding: 20px; border-radius: 10px;" markdown="block">

## 10. MEGR 2157 – Finite Element Analysis and Optimization – Kelsey Skipper

**[INSERT KELSEY'S MEGR 2157 DOCUMENTATION HERE]**

### 10.1 FEA Model Setup

[INSERT]

### 10.2 Boundary Conditions and Loading

[INSERT]

### 10.3 Mesh Refinement and Convergence

[INSERT]

### 10.4 FEA Results

| Parameter | Initial Design | Optimized Design |
|---|---|---|
| Maximum von Mises Stress | [INSERT] | [INSERT] |
| Maximum Vertical Deflection | [INSERT] | [INSERT] |
| Minimum Factor of Safety | [INSERT] | [INSERT] |
| Mass or Volume | [INSERT] | [INSERT] |

### 10.5 Design Optimization

[INSERT]

---

## 11. MEGR 2157 – Detailed Engineering Drawing – Kelsey Skipper

**[INSERT KELSEY'S ENGINEERING DRAWING DOCUMENTATION HERE]**

The detailed engineering drawing will include the crosshead geometry, third-angle projection views, dimensions, tolerances, and mounting interfaces.

### Required General Tolerances

| Decimal Precision | Tolerance |
|---|---|
| X.X | ±0.02 in |
| X.XX | ±0.01 in |
| X.XXX | ±0.005 in |

[INSERT ENGINEERING DRAWING IMAGE]

</div>

---

## 12. Project Time and Resources

The project involved engineering calculations, component research, CAD modeling, assembly development, analysis, and documentation.

| Task | Time |
|---|---|
| Research and Component Selection | [INSERT] |
| Lead Screw and Nut Calculations | [INSERT] |
| Crosshead Strength and Deflection Calculations | [INSERT] |
| Preliminary Engineering Sketch | [INSERT] |
| SolidWorks Crosshead Modeling | [INSERT] |
| SolidWorks Assembly | [INSERT] |
| FEA and Optimization | [INSERT] |
| Engineering Drawing | [INSERT] |
| Documentation | [INSERT] |
| **Total Project Time** | **[INSERT]** |

### Resources Used

- SolidWorks CAD
- McMaster-Carr
- Grainger
- Machinery's Handbook
- Engineering Mechanics course materials
- MEGR 2156 and MEGR 2157 lecture materials

---

## 13. Challenges and Lessons Learned

<div style="background-color: #DDF3E4; color: #243B2B; padding: 20px; border-radius: 10px;" markdown="block">

### Gracie Steelmon

**[INSERT GRACIE'S SPECIFIC CHALLENGES AND LESSONS LEARNED]**

</div>

<div style="background-color: #FCE3E3; color: #4A2424; padding: 20px; border-radius: 10px;" markdown="block">

### Kaileigh Hill

Through this project, I gained experience developing a mechanical assembly from engineering calculations and commercially available components.

One important lesson was understanding how individual component dimensions affect the overall assembly. The crosshead openings, lead screw spacing, and flange nut positioning all needed to be consistent for the components to align correctly.

I also gained experience using SolidWorks assembly mates to position mechanical components and represent their intended relationships.

Using manufacturer CAD files demonstrated how existing mechanical components can be incorporated into a custom engineering design while reducing unnecessary modeling work.

</div>

<div style="background-color: #E8F1FA; color: #243B53; padding: 20px; border-radius: 10px;" markdown="block">

### Kelsey Skipper

**[INSERT KELSEY'S SPECIFIC CHALLENGES AND LESSONS LEARNED]**

</div>

---

## 14. References

1. Machinery's Handbook, 31st Edition, Simple Mechanisms – Screws.
2. Machinery's Handbook, 31st Edition, Ball and Acme Lead Screws.
3. Engineering Mechanics, Chapter 6/5 – Screws.
4. [McMaster-Carr – Lead Screw](https://www.mcmaster.com/99030A993/)
5. [McMaster-Carr – Bronze Flange Nut](https://www.mcmaster.com/95120A592/)
6. [Grainger – T-Slot Framing](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48)
