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

![Parameter Table](YOUR-IMAGE-LINK)

### Creating the Model

I began creating the bracket using the parameters defined above instead of entering fixed dimensions. This allows changes to the parameters to automatically update the corresponding features of the model.

![Beginning CAD Model](YOUR-IMAGE-LINK)
