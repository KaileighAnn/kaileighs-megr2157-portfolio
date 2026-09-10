# A3 – Parametric and FEA

## Objective

The objective of this assignment is to design an aluminum bar using parametric CAD and then verify the design using Finite Element Analysis (FEA). I will use the given maximum deflection along with my chosen load, material properties, and cross-sectional dimensions to calculate the required length of the bar. I will then create the bar parametrically in SolidWorks and use FEA to compare the deflection and stress results with my calculations.

## Analyze

To begin the design, I chose the values I would use for the aluminum bar based on the requirements given in the assignment. I chose an applied load of **400 lbf**, which is within the required range of 300–500 lbf. I used a Young's Modulus of **10 × 10⁶ psi**, which is within the given range for aluminum, and a maximum allowable axial deflection of **0.009 in**.

### Initial Design Values

| Parameter | Value |
|---|---:|
| Material | Aluminum |
| Applied Load, F | 400 lbf |
| Maximum Deflection, δ | 0.009 in |
| Young's Modulus, E | 10 × 10⁶ psi |
| Diameter, d | 1.00 in |
| Yield Strength, Sy | 40 ksi |

I chose a circular cross section with a diameter of **1.00 in** for my initial design. I first calculated the cross-sectional area of the bar and then used the direct tension elongation equation to determine the required length.

### Hand Calculations

<p align="center">
  <img width="808" height="434" alt="image" src="https://github.com/user-attachments/assets/bbc457fc-24de-4262-8ffb-33e4fca004c3" />

</p>

<p align="center"><em>Figure 1. Hand calculations for the cross-sectional area and required bar length.</em></p>

From my calculations, the cross-sectional area of the bar is **0.7854 in²** and the required length is **176.71 in**. These values will be used to create the parametric model in SolidWorks. Instead of directly entering the calculated length, I will link the length to the design parameters so that the model will automatically update when one of the parameters is changed.

### Parametric SolidWorks Model

### Setting Up the Parametric Equations in SolidWorks

Before creating the bar, I set up global variables and equations in SolidWorks so the dimensions of the model could be controlled parametrically. I used the same values from my hand calculations for the diameter, applied load, maximum deflection, and Young's Modulus.

The cross-sectional area was defined using:

**A = πd² / 4**

The length was then calculated using the axial deflection equation rearranged for length:

**L = δEA / F**

I entered these relationships into the SolidWorks Equations, Global Variables, and Dimensions table. This allowed SolidWorks to calculate the required length instead of entering the length manually.

<p align="center">
 <img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/b2f2200e-8267-4df3-a875-878a4e63416a" />
</p>

<p align="center"><em>Figure 2. Global variables and equations used to parametrically determine the bar length in SolidWorks.</em></p>

SolidWorks calculated a bar length of **176.71 in**, which matches my hand-calculated value of **176.71 in**. This confirmed that the equations and parameters were entered correctly. The model can now update automatically when one of the design parameters is changed.

### Creating the Parametric Bar

After setting up the global variables and equations, I created the geometry of the bar in SolidWorks. I started by creating a circular sketch centered at the origin. Instead of manually entering the diameter, I linked the diameter dimension to the global variable **d**. This gave the bar a diameter of **1.00 in** and allows the diameter to update automatically if the parameter is changed.

<p align="center">
  <img width="960" height="600" alt="Circular sketch with parametric diameter" src="https://github.com/user-attachments/assets/31797338-7925-4c65-9741-4d521e197843" />
</p>

<p align="center"><em>Figure 3. Circular sketch with the diameter linked to the global variable d.</em></p>

Next, I used **Extruded Boss/Base** to create the bar. Instead of manually entering the calculated length, I linked the extrusion depth to the global variable **L**. SolidWorks used the parametric equation to determine the required bar length of **176.71 in**.

<p align="center">
  <img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/16a64687-7719-45da-8f38-52b929e0b954" />

</p>

<p align="center"><em>Figure 4. Completed parametric bar with a calculated length of 176.71 in.</em></p>

By linking the dimensions to the global variables, the geometry of the bar will automatically update when the design parameters are changed. This will allow me to test how changing different parameters affects the required length of the bar later in the assignment.

### Selecting the Aluminum Material

After creating the parametric bar, I assigned an aluminum material in SolidWorks so the finite element analysis would use realistic material properties. I selected **6061 Alloy** from the SolidWorks material library.

<p align="center">
  <img width="960" height="600" alt="6061 aluminum material properties in SolidWorks" src="https://github.com/user-attachments/assets/a8fdb3da-0f8e-4308-a3b4-3de801d4531a" />
</p>

<p align="center"><em>Figure 5. 6061 Alloy material properties selected in SolidWorks.</em></p>

The material library listed the Elastic Modulus as **6.9 × 10¹⁰ Pa**, which is approximately **10 × 10⁶ psi**. This closely matches the Young's Modulus value used in my hand calculations, so the material was appropriate for comparing the analytical and FEA results.

For the final safety factor calculation, I will use the assignment-specified aluminum yield strength of **40 ksi**.

### FEA Setup

After completing the parametric model and assigning the material, I used **SOLIDWORKS SimulationXpress** to perform the finite element analysis. I set up the analysis to represent the same direct tension loading condition used in my hand calculations.

#### Fixture

I first applied a fixed geometry fixture to one circular end of the bar. This prevents that end of the bar from moving and provides the reaction needed for the applied tensile load.

<p align="center">
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/b7f3d27c-b68a-4f0a-92d4-143ce71475e3" />
</p>

<p align="center"><em>Figure 6. Fixed geometry applied to one end of the aluminum bar.</em></p>

#### Applied Load

I then selected the circular face on the opposite end of the bar and applied a **400 lbf** force normal to the face. The direction of the force was reversed so that it pointed away from the fixed end, placing the bar in direct tension.

<p align="center">
<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/8d2d5136-898e-47a6-aadd-8e49b95b323a" />

</p>

<p align="center"><em>Figure 7. A 400 lbf tensile load applied normal to the opposite end of the bar.</em></p>

Using a fixed end and a 400 lbf axial load allows the FEA setup to represent the same loading conditions used in the axial deflection hand calculation.

### FEA Deflection Results

After setting up the fixture, 400 lbf tensile load, and aluminum material, I ran the analysis in SolidWorks SimulationXpress. I first looked at the displacement results to compare the FEA deflection to the maximum deflection used in my parametric design.

<p align="center">
<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/0b443b59-7e67-4eb7-a65f-6fe9d0fc9084" />
</p>

<p align="center"><em>Figure 8. FEA displacement map of the aluminum bar under a 400 lbf tensile load.</em></p>

The FEA showed a maximum resultant displacement of **0.2289 mm**, which converts to approximately **0.00901 in**. My parametric hand calculation used a maximum axial deflection of **0.00900 in**, so the two results are very close.

The deformation shown in the image is exaggerated by SolidWorks with a deformation scale of **1,960.67** so that the small change in length can be seen more clearly. The actual deformation of the bar is only about **0.009 in**.

### FEA von Mises Stress Results

Next, I viewed the von Mises stress results from the FEA to determine the maximum stress in the bar under the 400 lbf tensile load.

<p align="center">
<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/4fe2329c-8521-4566-ac9e-41d5319fd8c8" />
</p>

<p align="center"><em>Figure 9. von Mises stress map of the aluminum bar under a 400 lbf tensile load.</em></p>

The FEA reported a maximum von Mises stress of **3.876 × 10⁶ Pa**, or approximately **0.562 ksi**. The assignment specifies a yield strength of **40 ksi** for aluminum. Since the maximum stress is much lower than the yield strength, the bar remains below yielding under the applied load.

### Safety Factor

To check whether the bar would yield under the applied load, I compared the maximum von Mises stress from the FEA to the aluminum yield strength given in the assignment.

The safety factor was calculated using:

**n = Sy / σmax**

Using:

**Sy = 40 ksi**

**σmax = 0.562 ksi**

The resulting safety factor is:

**n = 40 / 0.562**

**n ≈ 71.2**

Since the safety factor is much greater than 1, the bar is well below the yield strength and passes the strength requirement for this loading condition.

SolidWorks displayed a different factor of safety because its built-in 6061 material uses a different yield strength than the **40 ksi** value specified in the assignment. For this report, I used the assignment-provided yield strength.

### Hand Calculation vs. FEA

The axial deflection from my hand calculation was **0.00900 in**. The FEA reported a maximum displacement of **0.2289 mm**, which is approximately **0.0090118 in**.

The percent difference between the two results was calculated using:

**Percent Difference = |FEA - Hand Calculation| / Hand Calculation × 100**

**Percent Difference = |0.0090118 - 0.00900| / 0.00900 × 100**

**Percent Difference ≈ 0.13%**

The two values are essentially the same. This is expected because the bar has a uniform cross section, the loading is purely axial, and there are no holes, notches, or other stress concentrations in the original geometry.

For this simple design, I would trust both results, but I would rely slightly more on the hand calculation because the geometry and loading match the assumptions of the axial deformation equation very closely. The FEA is still useful because it verifies that the CAD model behaves as expected.

### Hypothetical Pin Hole Stress Concentration

The assignment also asked me to consider how a substantial pin hole would affect the stress in the bar without rerunning the FEA. For this hypothetical case, I used a hole-to-width ratio of **d/W = 0.50**.

For a flat bar with a circular hole under axial tension, the stress concentration factor at this ratio is approximately:

**Kt ≈ 2.16**

Using the nominal stress from my FEA:

**σnominal = 0.562 ksi**

The estimated peak stress at the edge of the hole is:

**σpeak = Kt × σnominal**

**σpeak = (2.16)(0.562 ksi)**

**σpeak ≈ 1.21 ksi**

Using the assignment-specified aluminum yield strength of **40 ksi**, the estimated safety factor is:

**n = 40 ksi / 1.21 ksi**

**n ≈ 33.1**

Even with the added stress concentration from the hypothetical pin hole, the estimated peak stress is still well below the aluminum yield strength, so the design would still pass the safety factor check.

## Design Reflection

The parametric design and FEA gave very similar results for the bar. My hand calculation was based on a maximum deflection of **0.00900 in**, while the FEA resulted in approximately **0.00901 in**. The percent difference was only about **0.13%**, which showed that the parametric equation and SolidWorks simulation agreed very closely.

I expected the results to be similar because the bar has a constant cross section and is only being loaded in direct tension. There are no changes in geometry or stress concentrations in the original design that would make the analysis more complicated. For this design, I would trust the hand calculation slightly more because the geometry and loading closely match the assumptions of the axial deflection equation. However, the FEA was useful for verifying my calculations and showing how the stress and displacement were distributed throughout the bar.

The FEA also showed a maximum von Mises stress of approximately **0.562 ksi**, which was much lower than the given aluminum yield strength of **40 ksi**. Overall, the results showed that the bar met both the deflection and strength requirements.

## 2157 Portion: Variable Changes

For the 2157 portion of the assignment, I changed the design parameters to see how they affected the calculated length of the bar. Before making the changes, I predicted whether the length would increase, decrease, or stay the same.

### Original Design

The original design used:

- **Applied Load, F = 400 lbf**
- **Diameter, d = 1.00 in**
- **Maximum Deflection, δ = 0.009 in**
- **Young's Modulus, E = 10 × 10⁶ psi**
- **Calculated Length, L = 176.71 in**

### Changing the Design Parameters

For the modified design, I changed the applied load to **450 lbf** and the diameter to **0.75 in**.

Before calculating the new length, I predicted that the required length would **decrease**. Increasing the applied load should decrease the allowable length, and decreasing the diameter reduces the cross-sectional area, which should also decrease the calculated length.

The new cross-sectional area was:

**A = πd² / 4**

**A = π(0.75)² / 4**

**A ≈ 0.4418 in²**

The new length was then calculated using:

**L = δEA / F**

**L = (0.009)(10,000,000)(0.4418) / 450**

**L ≈ 88.36 in**

<p align="center">
<img width="598" height="261" alt="image" src="https://github.com/user-attachments/assets/83aaceab-4b68-4103-bb3c-3687e285484d" />
</p>

<p align="center"><em>Figure 10. Updated SolidWorks equations after changing the applied load and diameter.</em></p>

After the parameters were changed, SolidWorks automatically recalculated the bar length from **176.71 in** to approximately **88.36 in**. This matched my prediction that the required length would decrease.

This showed how the parametric model can automatically update the geometry when the design variables are changed without manually recalculating or rebuilding the entire model.
## Lessons Learned

This assignment helped me better understand how parametric modeling can be used to connect engineering calculations directly to CAD geometry. Instead of manually entering the bar length, I used equations in SolidWorks so the model could automatically update when the design variables changed.

I also learned more about using SimulationXpress for a basic FEA. The displacement and von Mises stress results helped verify that my hand calculations were reasonable and that the bar stayed well below the aluminum yield strength.

One thing that confused me at first was the exaggerated deformation shown in the FEA animation. The visual deformation looked much larger than the actual displacement because SolidWorks increased the deformation scale to make the change easier to see. I also had to make sure the force direction was correct so the bar was in tension rather than compression.

Overall, the biggest thing I learned was how hand calculations, parametric CAD, and FEA can all be used together to check the same design.

### Mistakes Made

One mistake I made was initially questioning whether the exaggerated deformation shown by SolidWorks represented the actual displacement. After reviewing the results, I realized the deformation was only visually scaled and the actual displacement was approximately **0.009 in**.

I also had to double-check the material properties and safety factor because the yield strength included in the SolidWorks 6061 material library was different from the **40 ksi** yield strength specified in the assignment.

### Time Spent

The total time I spent completing this assignment was approximately **4 hours** from start to finish. This included the hand calculations, setting up the parametric equations, creating the CAD model, running the FEA, analyzing the results, and documenting everything in my portfolio.

## CAD File Download

The completed SolidWorks CAD model for this assignment can be downloaded below.

[**Click here to download the A3 Parametric Bar CAD file**](https://onedrive.live.com/personal/0D789EE8B59210B1/_layouts/15/download.aspx?SourceUrl=%2Fpersonal%2F0D789EE8B59210B1%2FDocuments%2FA3P%2ESLDPRT)
