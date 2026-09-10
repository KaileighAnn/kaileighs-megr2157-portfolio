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

## Decide

<!-- We will add the comparison between the hand calculations and FEA results here. -->

## Communicate

<!-- We will add the design reflection, lessons learned, mistakes, and time spent here. -->

## 2157 Portion: Variable Changes

<!-- We will change the design parameters one at a time and document the results here. -->

## CAD File Download

<!-- IMPORTANT: Add the downloadable SolidWorks CAD file here before submission. -->
