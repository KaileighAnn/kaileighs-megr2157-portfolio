# A06 – Design for Strength and Stiffness II

## Objective

The objective of this assignment is to continue the bracket design from the previous assignment by creating a parametric CAD model and a fully dimensioned engineering drawing.

The dimensions determined from the previous strength and stiffness analyses will be used to control the bracket geometry. The final drawing will include appropriate tolerances to ensure the bracket properly fits the rigid T-beam.

## Previous Design

In the previous assignment, the bracket was analyzed using both strength and stiffness. Five features, labeled A through E, were analyzed individually to determine the required dimensions.

Stress governed the final design for all five features, so the dimensions selected from the stress analysis will be used as the starting dimensions for the parametric CAD model.

## Design Requirements

- Use the dimensions determined from the previous strength and stiffness analysis.
- Create a parametric solid model of the bracket.
- Show the CAD parameter table.
- Drive at least one model dimension directly using an analytical equation.
- Create a fully dimensioned multiview engineering drawing.
- Use third-angle projection.
- Apply appropriate tolerances to the three sliding-fit interfaces with the rigid T-beam.
- Include a tolerance block:
  - X.X ± .02
  - X.XX ± .01
  - X.XXX ± .005
- Export the finished drawing as a PDF.
- Provide a download link to the finished CAD files.

## Parametric Design

### Starting Dimensions

The final dimensions from the previous assignment were used as the starting point for the parametric bracket model.

| Feature | Dimension | Selected Value |
|---|---|---:|
| A | Diameter, d_A | 0.875 in |
| B | Thickness, t_B | 0.150 in |
| C | Width, w_C | 1.375 in |
| D | Thickness, t_D | 0.050 in |
| E | Thickness, t_E | 1.375 in |

## CAD Model

### Parameter Setup

Before creating the bracket, I created parameters for the important dimensions of the design. This allows the dimensions to be controlled from one location and allows the model to update automatically if a parameter changes.

The starting values were based on the final dimensions selected from the strength and stiffness analysis in the previous assignment.

<img width="605" height="415" alt="image" src="https://github.com/user-attachments/assets/6954d8db-0d4d-4e34-b370-cc6b5344e6a7" />

### Creating the Model

I began creating the bracket using the parameters defined above instead of entering fixed dimensions. This allows changes to the parameters to automatically update the corresponding features of the model.

<img width="627" height="409" alt="image" src="https://github.com/user-attachments/assets/184e0253-6db6-4b20-8027-3145374f559b" />

<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/40281d42-9f57-493e-beb6-5785e50710b8" />

<img width="1345" height="867" alt="image" src="https://github.com/user-attachments/assets/a384689b-5691-4cf6-aa1a-1e9ace182bf2" />

<img width="1177" height="850" alt="image" src="https://github.com/user-attachments/assets/b550359d-22bd-4dc8-8c59-ee926c64e83d" />

<img width="787" height="808" alt="image" src="https://github.com/user-attachments/assets/1974c8fd-0b64-46f8-8d6b-f2148980617c" />

## Engineering Drawing

After completing the parametric CAD model, I created a multiview engineering drawing of the bracket. The drawing uses third-angle projection and includes front, top, and right-side views along with an isometric view.

The drawing was dimensioned to communicate the geometry needed to manufacture the bracket and assemble it with the rigid T-beam. Tighter tolerances were applied to functional mating features, while less critical dimensions were allowed to use the general tolerances in the tolerance block.

### Third-Angle Multiview Drawing

The front, top, and right-side views were arranged using third-angle projection. An isometric view was also included to make the overall bracket geometry easier to interpret.

<img width="509" height="368" alt="image" src="https://github.com/user-attachments/assets/aed81547-1d32-4f02-bc90-4104e1e891b9" />

### Tolerances

The following general tolerance block was included on the engineering drawing:

- X.X ± .02 in
- X.XX ± .01 in
- X.XXX ± .005 in

Tighter tolerances were used on the sliding-fit interfaces because these dimensions directly affect how the bracket fits over the rigid T-beam. Non-critical dimensions were given looser tolerances where possible to avoid unnecessarily restricting manufacturing.

### Analytical Equation

The allowable stress used for the design was determined from the yield strength and safety factor:

**σ_allow = σ_y / SF**

**σ_allow = 40,000 psi / 4 = 10,000 psi**

The design equations from A05 were used to determine the required dimensions of the bracket. These dimensions were then incorporated into the SolidWorks parameter table to control the model geometry.

## Mistakes and Design Changes

During the modeling process, I initially had difficulty connecting the calculated A05 dimensions to the correct bracket features. I corrected the parameter setup and rebuilt portions of the sketch so that the important dimensions were controlled parametrically.

I also adjusted the drawing setup to clearly show the front, top, right-side, and isometric views and added the required tolerance information.

## Reflections

### Parametric Design

One lesson I learned was how analytical design calculations can be incorporated into a parametric CAD model. Instead of treating the calculations and CAD model as separate steps, parameters and equations allow the geometry to respond to engineering requirements.

Using global variables also made the design easier to modify because important dimensions could be controlled from one location instead of manually changing multiple sketches and features.

### Dimensioning and Tolerancing

The sliding-fit dimensions require tighter tolerances because they control the interface between the bracket and the rigid T-beam. A small dimensional error at these surfaces could prevent the parts from assembling or could create excessive clearance.

Non-critical dimensions can use looser tolerances because small variations do not significantly affect the function of the bracket. Applying unnecessarily tight tolerances to non-critical dimensions can increase manufacturing difficulty and cost without improving the function of the part.

## Time Spent

The total time spent completing the parametric model, engineering drawing, documentation, and revisions was approximately **6 hours**.

## CAD Files

The completed SolidWorks files and engineering drawing can be downloaded below:

[A6_Bracket.zip](https://github.com/user-attachments/files/32888813/A6_Bracket.zip)

## 2157 – Link Design

### Design

A link was designed to connect with the previously designed bracket. The link was analyzed for both strength and stiffness before being modeled parametrically in SolidWorks.

The final link dimensions were selected so that the link satisfied both the required minimum cross-sectional area and maximum allowable deflection.

## Parametric Design

The link was modeled parametrically in SolidWorks using global variables for the important dimensions.

| Parameter | Value |
|---|---:|
| Link Length | 3.00 in |
| Link Width | 1.50 in |
| Link Thickness | 0.25 in |
| Top Hole Diameter | 1.00 in |
| Bottom Hole Diameter | 0.875 in |

Using parameters allows the important link dimensions to be controlled from one location and makes later design changes easier.

### CAD Model

The final link is 3.00 in long, 1.50 in wide, and 0.25 in thick. The link contains a Ø1.00 in top hole and Ø0.875 in bottom hole.

Both holes were centered along the longitudinal centerline of the link.

<img width="1216" height="1294" alt="image" src="https://github.com/user-attachments/assets/81ee4d5e-8986-4e85-9e3d-16fef8b51bf1" />

### Tolerancing and GD&T

Tighter tolerances were applied to the holes because these features control how the link interfaces with other components.

The top hole was specified as **Ø1.000 ± .005 in**, and the bottom hole was specified as **Ø0.875 ± .010 in**.

A primary flat surface was identified as Datum A. A perpendicularity control was applied to a critical hole axis relative to Datum A to communicate the required orientation of the mating feature.

The general tolerance block used on the drawing was:

- X.X ± .02
- X.XX ± .01
- X.XXX ± .005

A drawing note identifies the hole that interfaces with the bracket.

## Link Reflection

This design showed how tolerances affect compatibility between mating parts. The hole dimensions need tighter control because dimensional variation at an interface can affect whether the components assemble correctly.

Dimensioning and tolerancing also communicate design intent. Critical mating features receive tighter tolerances and geometric controls, while non-critical dimensions can use the general tolerance block. This provides the information needed to manufacture the part without unnecessarily restricting every dimension.


