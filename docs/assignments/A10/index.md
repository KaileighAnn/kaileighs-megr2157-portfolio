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


<h1>A10 – Lead Screw Translating System Design</h1>

<h2>Group Members</h2>

<ul>
<li><strong>Gracie Steelmon</strong> – Lead Screw and Crosshead Calculations</li>
<li><strong>Kaileigh Hill</strong> – Parametric Modeling and CAD Assembly</li>
<li><strong>Kelsey Skipper</strong> – MEGR 2157 Analysis and Documentation</li>
</ul>

<hr>

<h2>Project Objective</h2>

<p>
The objective of this project was to conceptually design a mechanically
driven tensile testing system capable of applying a controlled axial
tensile load of up to <strong>2 kN</strong> to a material specimen.
</p>

<p>
A tensile tester is used to evaluate the mechanical properties of
materials by applying a controlled pulling force and measuring the
resulting deformation. This allows engineers to determine material
properties such as yield strength, ultimate tensile strength, and
elongation at failure.
</p>

<p>
Our proposed design uses two Acme lead screws to translate a crosshead
vertically, allowing a tensile force to be applied to the specimen.
The system was designed to emphasize structural strength, controlled
movement, proper component alignment, and minimal crosshead deflection.
</p>

<h3>Design Requirements</h3>

<table>
<thead>
<tr>
<th>Design Parameter</th>
<th>Requirement</th>
</tr>
</thead>
<tbody>
<tr><td>Maximum Tensile Load</td><td>2 kN</td></tr>
<tr><td>Crosshead Speed</td><td>1–50 mm/min</td></tr>
<tr><td>Minimum Lead Screw Length</td><td>18 in</td></tr>
<tr><td>Number of Lead Screws</td><td>2</td></tr>
<tr><td>Required Safety Factor</td><td>4</td></tr>
<tr><td>Maximum Crosshead Deflection</td><td>0.1 mm</td></tr>
<tr><td>Operating System</td><td>Fully Mechanical</td></tr>
<tr><td>Configuration</td><td>Bench-Top Tensile Tester</td></tr>
</tbody>
</table>

<h3>Project Scope</h3>

<ol>
<li>Determine the minimum lead screw diameter using axial stress analysis.</li>
<li>Calculate the required lead screw rotational speed range.</li>
<li>Determine the torque required to produce the specified tensile load.</li>
<li>Select appropriate Acme lead screws and bronze flange nuts.</li>
<li>Analyze crosshead strength and deflection.</li>
<li>Develop a preliminary multiview crosshead sketch.</li>
<li>Tabulate the costs of commercially available components.</li>
<li>Create a SolidWorks model and assembly of the proposed tensile tester.</li>
<li>Perform additional FEA and engineering drawing work for MEGR 2157.</li>
</ol>

<p>
The overall goal was to develop a mechanically feasible tensile tester
design that could provide consistent loading while maintaining
structural integrity and alignment.
</p>

<hr>

<!-- ============================================ -->
<!-- GRACIE STEELMON - GREEN SECTION -->
<!-- ============================================ -->

<div style="background-color: #DDF3E4; color: #243B2B; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h2>1. Lead Screw Diameter Analysis – Gracie Steelmon</h2>

<h3>1.1 Minimum Lead Screw Diameter</h3>

<p>
The minimum diameter of the lead screws was determined using axial
stress analysis.
</p>

<p>
Because the tensile tester uses two identical lead screws, the applied
2 kN tensile load was assumed to be distributed equally between them.
</p>

<p>
The force supported by each lead screw was therefore:
</p>

<p><strong>Force per Lead Screw = 1,000 N</strong></p>

<p>
A safety factor of 4 was applied when determining the minimum
acceptable screw diameter.
</p>

<p>
The analysis included identifying the known and unknown variables,
developing a free-body diagram, solving the governing equations
symbolically, and calculating the required diameter numerically.
</p>

<img width="1904" height="2540" alt="image" src="https://github.com/user-attachments/assets/0bc8769c-7e0f-414c-87d1-cb67aca92aaa" />

<p><em>Figure 1: Axial stress analysis used to determine the minimum lead screw diameter.</em></p>

<hr>

<h2>2. Lead Screw Rotational Speed – Gracie Steelmon</h2>

<h3>2.1 Rotational Speed Range</h3>

<p>
The required rotational speed range was determined using the specified
crosshead translation speed of 1–50 mm/min.
</p>

<p>
The relationship between linear translation and rotational speed
depends on the lead of the selected screw.
</p>

<p>
For a lead screw, the linear translation per revolution is equal
to the screw lead.
</p>

<p><strong>Linear Speed = Rotational Speed × Screw Lead</strong></p>

<p>Rearranging:</p>

<p><strong>Rotational Speed = Linear Speed / Screw Lead</strong></p>

<p>
The calculations were used to determine the rotational speeds
necessary to achieve the required crosshead movement.
</p>

<img width="1844" height="2364" alt="image" src="https://github.com/user-attachments/assets/5793dd42-ea1c-4d6d-a522-5dc81a2d18b7" />

<p><em>Figure 2: Calculations determining the required lead screw rotational speed range.</em></p>

<hr>

<h2>3. Lead Screw Torque and Selection – Gracie Steelmon</h2>

<h3>3.1 Maximum Torque Analysis</h3>

<p>
The maximum torque required to produce the specified 2 kN tensile
load was determined using lead screw mechanics.
</p>

<p>
This analysis considered the relationship between rotational input
torque and the resulting axial force.
</p>

<p>
The torque requirement is influenced by the applied load, screw
geometry, thread friction, and lead angle.
</p>

<p>
The calculations were used to evaluate the torque required to
operate the proposed system.
</p>

<img width="1820" height="2368" alt="image" src="https://github.com/user-attachments/assets/9f676d49-c27e-41a1-a888-4aa0584f988e" />

<p><em>Figure 3: Torque analysis used to evaluate and select the lead screws.</em></p>

<h3>3.2 Final Lead Screw Selection</h3>

<p>
The selected component was a <strong>right-hand, 3/8"-12 Acme lead screw</strong>,
specified as 1018 carbon steel in the original selection notes.
</p>

<p>
A 3-foot length was selected because the alternative 18-inch length
was insufficient for the proposed design.
</p>

<p>
The longer screw provides additional material for cutting to the
required assembly length.
</p>

<table>
<thead>
<tr><th>Feature</th><th>Specification</th></tr>
</thead>
<tbody>
<tr><td>Thread Type</td><td>Acme</td></tr>
<tr><td>Thread Size</td><td>3/8"-12</td></tr>
<tr><td>Thread Direction</td><td>Right-Hand</td></tr>
<tr><td>Material</td><td>Carbon Steel – Grade to Verify</td></tr>
<tr><td>Purchased Length</td><td>3 ft</td></tr>
<tr><td>Quantity</td><td>2</td></tr>
</tbody>
</table>

<p>
<a href="https://www.mcmaster.com/99030A993/" target="_blank">
McMaster-Carr Lead Screw
</a>
</p>

<p>
<strong>Material Verification:</strong> The original selection notes
specify 1018 carbon steel, while the initial cost table lists 1080
carbon steel. The material grade should be confirmed using the
selected supplier part number.
</p>

<hr>

<h2>4. Bronze Nut and Flange Selection – Gracie Steelmon</h2>

<h3>4.1 Internal Thread Analysis</h3>

<p>
The bronze flange nuts were selected to support the axial loading
transmitted through the lead screws.
</p>

<p>
Thread bending stress analysis was performed to evaluate whether
the internal threads could withstand the applied load while
satisfying the required safety factor.
</p>

<p>
The analysis included identifying the known and unknown variables,
developing a free-body diagram, solving the governing equations
symbolically, and calculating the thread bending stress numerically.
</p>

<img width="1800" height="2408" alt="image" src="https://github.com/user-attachments/assets/b9c1b330-5509-4edb-b046-5df9507ad84a" />

<p><em>Figure 4: Internal thread analysis used to evaluate the bronze flange nut.</em></p>

<h3>4.2 Selected Component</h3>

<table>
<thead>
<tr><th>Feature</th><th>Specification</th></tr>
</thead>
<tbody>
<tr><td>Component</td><td>Acme Bronze Flange Nut</td></tr>
<tr><td>Thread Size</td><td>3/8"-12</td></tr>
<tr><td>Thread Direction</td><td>Right-Hand</td></tr>
<tr><td>Material</td><td>Bearing Bronze</td></tr>
<tr><td>Quantity</td><td>2</td></tr>
</tbody>
</table>

<p>
<a href="https://www.mcmaster.com/95120A592/" target="_blank">
McMaster-Carr Bronze Flange Nut
</a>
</p>

<hr>

<h2>5. Crosshead Stress and Strength Analysis – Gracie Steelmon</h2>

<h3>5.1 Beam Strength Analysis</h3>

<p>
The crosshead was designed to transfer the tensile testing load
between the two lead screws while maintaining structural integrity.
</p>

<p>
Simple beam stress and strength calculations were used to evaluate
the required crosshead dimensions and material.
</p>

<p>
The analysis considered the applied loading, support locations,
bending stress, and required safety factor.
</p>

<p>
The crosshead was treated as a structural member subjected to
loading from the tensile specimen and supported at the lead
screw locations.
</p>

<img width="1820" height="2356" alt="image" src="https://github.com/user-attachments/assets/34af6662-71ff-4374-9932-6b10a0f673f6" />

<p><em>Figure 5: Beam stress and strength analysis for the tensile tester crosshead.</em></p>

<hr>

<h2>6. Crosshead Beam Deflection Analysis – Gracie Steelmon</h2>

<h3>6.1 Deflection Requirements</h3>

<p>
The crosshead was evaluated for vertical deflection under the
applied 2 kN tensile load.
</p>

<p>
The maximum allowable deflection was specified as
<strong>0.1 mm</strong>.
</p>

<p>
Beam deflection equations were used to evaluate the relationship
between material stiffness, crosshead geometry, and applied loading.
</p>

<p>
The analysis helped establish the crosshead dimensions necessary
to limit bending during tensile testing.
</p>

<img width="1836" height="2408" alt="image" src="https://github.com/user-attachments/assets/f723f418-93d1-4be7-bb61-61c2c73579ab" />

<p><em>Figure 6: Beam deflection calculations used to evaluate crosshead stiffness.</em></p>

<hr>

<h2>7. Crosshead Multiview Sketch – Gracie Steelmon</h2>

<h3>7.1 Preliminary Crosshead Design</h3>

<p>
A preliminary multiview sketch was created to communicate the
proposed crosshead geometry.
</p>

<p>
The sketch includes the overall dimensions, lead screw locations,
and mounting features required for the bronze flange nuts.
</p>

<p>
The purpose of the sketch was to establish the initial geometry
before creating the SolidWorks model.
</p>

<img src="multiviewsketch.jpg" width="900" style="max-width:100%; height:auto;" alt="Crosshead Multiview Sketch">

<p><em>Figure 7: Preliminary multiview engineering sketch of the crosshead.</em></p>

</div>

<hr>

<h2>8. Material Cost Analysis</h2>

<p>
The cost of the commercially available mechanical components was
estimated using supplier pricing.
</p>

<p>
The following table includes the selected components, quantities,
individual prices, and total estimated costs.
</p>

<table>
<thead>
<tr>
<th>Item</th>
<th>Quantity</th>
<th>Component</th>
<th>Cost per Item</th>
<th>Total Cost</th>
<th>Purchase Link</th>
</tr>
</thead>
<tbody>
<tr>
<td>1</td>
<td>2</td>
<td>Carbon Steel Acme Lead Screw, RH, 3/8"-12, 3 ft</td>
<td>$35.32</td>
<td>$70.64</td>
<td><a href="https://www.mcmaster.com/99030A993/">McMaster-Carr</a></td>
</tr>
<tr>
<td>2</td>
<td>2</td>
<td>Acme Bronze Flange Nut, RH, 3/8"-12</td>
<td>$111.78</td>
<td>$223.56</td>
<td><a href="https://www.mcmaster.com/95120A592/">McMaster-Carr</a></td>
</tr>
<tr>
<td>3</td>
<td>1</td>
<td>T-Slot Framing System</td>
<td>$245.87</td>
<td>$245.87</td>
<td><a href="https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48">Grainger</a></td>
</tr>
<tr>
<td colspan="4"><strong>Total Estimated Cost</strong></td>
<td><strong>$540.07</strong></td>
<td></td>
</tr>
</tbody>
</table>

<p>
The total estimated purchased component cost was
<strong>$540.07</strong>, excluding custom-fabricated parts,
machining, and other unlisted hardware.
</p>

<hr>

<!-- ============================================ -->
<!-- KAILEIGH HILL - RED SECTION -->
<!-- ============================================ -->

<div style="background-color: #FCE3E3; color: #4A2424; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h2>9. Parametric Modeling and CAD Assembly – Kaileigh Hill</h2>

<h3>Objective</h3>

<p>
The objective of my portion of this project was to create a 3D
CAD model of the tensile tester using SolidWorks.
</p>

<p>
I modeled the crosshead and assembled the selected lead screws,
bronze flange nuts, and framing components.
</p>

<p>
The goal was to create an assembly that represents how the
mechanical components fit together using the dimensions
established through our team's calculations.
</p>

<h3>9.1 Crosshead Modeling</h3>

<p>
I began by creating the crosshead in SolidWorks using the
dimensions determined through our team's calculations.
</p>

<p>
I sketched a rectangular profile and used the Extruded Boss/Base
feature to create the initial solid.
</p>

<p>
Next, I created two circular openings for the lead screws
and bronze flange nuts.
</p>

<p>
The openings were positioned symmetrically near each end of
the crosshead and created using the Extruded Cut feature.
</p>

<h4>Crosshead Dimensions</h4>

<table>
<thead>
<tr><th>Feature</th><th>Dimension</th></tr>
</thead>
<tbody>
<tr><td>Length</td><td>12.00 in</td></tr>
<tr><td>Width</td><td>3.00 in</td></tr>
<tr><td>Height</td><td>3.684 in</td></tr>
<tr><td>Lead Screw Opening Diameter</td><td>0.510 in</td></tr>
<tr><td>Lead Screw Center Spacing</td><td>10.00 in</td></tr>
<tr><td>Material</td><td>A36 Low Carbon Steel</td></tr>
</tbody>
</table>

<img width="960" style="max-width:100%; height:auto;" alt="Initial Crosshead Model" src="https://github.com/user-attachments/assets/dde21ab3-a162-4c19-b113-25595c0aabb6">

<p><em>Figure 8: Initial SolidWorks crosshead model before adding the lead screw openings.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Completed Crosshead Model" src="https://github.com/user-attachments/assets/c9d4eb3e-d79a-4626-9064-69ef4d9a6c7d">

<p><em>Figure 9: Completed crosshead model showing the two lead screw openings.</em></p>

<hr>

<h3>9.2 Downloading CAD Components</h3>

<p>
After modeling the crosshead, I downloaded the manufacturer
CAD files for the lead screws and bronze flange nuts from
McMaster-Carr.
</p>

<p>
Using existing CAD files allowed me to incorporate accurate
component geometry without modeling commercially available
parts from scratch.
</p>

<h4>Components Included</h4>

<ul>
<li>Two 3/8"-12 Acme lead screws specified as 1018 carbon steel in the original selection notes.</li>
<li>Two 3/8"-12 Acme flange nuts made from 932 bearing bronze.</li>
<li>T-slot framing components obtained from Grainger.</li>
</ul>

<h4>Component Links</h4>

<ul>
<li><a href="https://www.mcmaster.com/99030A993/">Acme Lead Screw – McMaster-Carr</a></li>
<li><a href="https://www.mcmaster.com/95120A592/">Bronze Flange Nut – McMaster-Carr</a></li>
<li><a href="https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48">T-Slot Framing – Grainger</a></li>
</ul>

<img width="960" style="max-width:100%; height:auto;" alt="Bronze Flange Nut" src="https://github.com/user-attachments/assets/67b3ee42-274f-4259-9dd5-ecd0a2453d9f">

<p><em>Figure 10: Manufacturer CAD model of the bronze Acme flange nut.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Acme Lead Screw" src="https://github.com/user-attachments/assets/62e8d474-b98e-4cfc-9dce-502b1d3796c5">

<p><em>Figure 11: Manufacturer CAD model of the 3/8"-12 Acme lead screw.</em></p>

<hr>

<h3>9.3 SolidWorks Assembly</h3>

<p>
After obtaining the necessary CAD components, I created
a new assembly in SolidWorks.
</p>

<p>
I inserted the crosshead first and used it as the reference
component for the assembly.
</p>

<p>
I then inserted two bronze flange nuts and aligned them with
the crosshead openings using Concentric Mates.
</p>

<p>
Coincident Mates were used to position the flange surfaces
against the crosshead.
</p>

<p>
The nuts were oriented with the flanges underneath the crosshead
to establish a direct load path for the proposed downward
tensile loading arrangement.
</p>

<p>
Next, I inserted two Acme lead screws and aligned them
with their corresponding flange nuts.
</p>

<p>
Finally, I incorporated the framing components into the
assembly to represent the overall tensile tester structure.
</p>

<img width="960" style="max-width:100%; height:auto;" alt="Crosshead and Flange Nuts" src="https://github.com/user-attachments/assets/3d28f4ba-af76-4e79-ae5c-d5eaef791a7f">

<p><em>Figure 12: Crosshead assembly showing both bronze flange nuts positioned underneath the crosshead.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Lead Screw Assembly" src="https://github.com/user-attachments/assets/d78998ab-44d5-4194-861c-32d321561d8b">

<p><em>Figure 13: SolidWorks assembly showing the lead screws aligned with the crosshead and bronze flange nuts.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Overall Tensile Tester Assembly" src="https://github.com/user-attachments/assets/f0d4743e-ddaa-48bc-950b-b4cef81cd20d">

<p><em>Figure 14: Overall SolidWorks CAD assembly of the tensile tester.</em></p>

<hr>

<h3>9.4 CAD Files</h3>

<p>
The SolidWorks CAD files for this project are available
in the downloadable ZIP folder below.
</p>

<p>
<strong>
<a href="https://github.com/user-attachments/files/34669260/Assem2.zip">
Download SolidWorks CAD Files
</a>
</strong>
</p>

<p>
The folder includes the crosshead, lead screws, bronze flange
nuts, framing components, and overall assembly.
</p>

</div>

<hr>

<!-- ============================================ -->
<!-- KELSEY SKIPPER - BLUE SECTION -->
<!-- ============================================ -->

<div style="background-color: #E8F1FA; color: #243B53; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h2>10. MEGR 2157 – Finite Element Analysis and Optimization – Kelsey Skipper</h2>

<p><strong>[INSERT KELSEY'S MEGR 2157 DOCUMENTATION HERE]</strong></p>

<h3>10.1 FEA Model Setup</h3>

<p>[INSERT MODEL SETUP AND MATERIAL PROPERTIES]</p>

<h3>10.2 Boundary Conditions and Loading</h3>

<p>[INSERT BOUNDARY CONDITIONS AND 2 kN LOAD APPLICATION]</p>

<h3>10.3 Mesh Refinement and Convergence</h3>

<p>[INSERT MESH REFINEMENT RESULTS AND IMAGES]</p>

<h3>10.4 FEA Results</h3>

<table>
<thead>
<tr>
<th>Parameter</th>
<th>Initial Design</th>
<th>Optimized Design</th>
</tr>
</thead>
<tbody>
<tr><td>Maximum von Mises Stress</td><td>[INSERT]</td><td>[INSERT]</td></tr>
<tr><td>Maximum Vertical Deflection</td><td>[INSERT]</td><td>[INSERT]</td></tr>
<tr><td>Minimum Factor of Safety</td><td>[INSERT]</td><td>[INSERT]</td></tr>
<tr><td>Mass or Volume</td><td>[INSERT]</td><td>[INSERT]</td></tr>
</tbody>
</table>

<h3>10.5 Design Optimization</h3>

<p>[INSERT OPTIMIZATION RESULTS AND DISCUSSION]</p>

<hr>

<h2>11. MEGR 2157 – Detailed Engineering Drawing – Kelsey Skipper</h2>

<p>
The detailed engineering drawing will include the crosshead
geometry, third-angle projection views, dimensions, tolerances,
and mounting interfaces.
</p>

<h3>Required General Tolerances</h3>

<table>
<thead>
<tr><th>Decimal Precision</th><th>Tolerance</th></tr>
</thead>
<tbody>
<tr><td>X.X</td><td>±0.02 in</td></tr>
<tr><td>X.XX</td><td>±0.01 in</td></tr>
<tr><td>X.XXX</td><td>±0.005 in</td></tr>
</tbody>
</table>

<p><strong>[INSERT ENGINEERING DRAWING IMAGE]</strong></p>

</div>

<hr>

<h2>12. Project Time and Resources</h2>

<p>
The project involved engineering calculations, component
research, CAD modeling, assembly development, analysis,
and documentation.
</p>

<table>
<thead>
<tr><th>Task</th><th>Time</th></tr>
</thead>
<tbody>
<tr><td>Research and Component Selection</td><td>[INSERT]</td></tr>
<tr><td>Lead Screw and Nut Calculations</td><td>[INSERT]</td></tr>
<tr><td>Crosshead Strength and Deflection Calculations</td><td>[INSERT]</td></tr>
<tr><td>Preliminary Engineering Sketch</td><td>[INSERT]</td></tr>
<tr><td>SolidWorks Crosshead Modeling</td><td>[INSERT]</td></tr>
<tr><td>SolidWorks Assembly</td><td>[INSERT]</td></tr>
<tr><td>FEA and Optimization</td><td>[INSERT]</td></tr>
<tr><td>Engineering Drawing</td><td>[INSERT]</td></tr>
<tr><td>Documentation</td><td>[INSERT]</td></tr>
<tr>
<td><strong>Total Project Time</strong></td>
<td><strong>[INSERT]</strong></td>
</tr>
</tbody>
</table>

<h3>Resources Used</h3>

<ul>
<li>SolidWorks CAD</li>
<li>McMaster-Carr</li>
<li>Grainger</li>
<li>Machinery's Handbook</li>
<li>Engineering Mechanics course materials</li>
<li>MEGR 2156 and MEGR 2157 lecture materials</li>
</ul>

<hr>

<h2>13. Challenges and Lessons Learned</h2>

<div style="background-color: #DDF3E4; color: #243B2B; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h3>Gracie Steelmon</h3>

<p><strong>[INSERT GRACIE'S SPECIFIC CHALLENGES AND LESSONS LEARNED]</strong></p>

</div>

<div style="background-color: #FCE3E3; color: #4A2424; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h3>Kaileigh Hill</h3>

<p>
Through this project, I gained experience developing a mechanical
assembly from engineering calculations and commercially available
components.
</p>

<p>
One important lesson was understanding how individual component
dimensions affect the overall assembly. The crosshead openings,
lead screw spacing, and flange nut positioning all needed to be
consistent for the components to align correctly.
</p>

<p>
I also gained experience using SolidWorks assembly mates to
position mechanical components and represent their intended
relationships.
</p>

<p>
Using manufacturer CAD files demonstrated how existing mechanical
components can be incorporated into a custom engineering design
while reducing unnecessary modeling work.
</p>

</div>

<div style="background-color: #E8F1FA; color: #243B53; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h3>Kelsey Skipper</h3>

<p><strong>[INSERT KELSEY'S SPECIFIC CHALLENGES AND LESSONS LEARNED]</strong></p>

</div>

<hr>

<h2>14. References</h2>

<ol>
<li>Machinery's Handbook, 31st Edition, Simple Mechanisms – Screws.</li>
<li>Machinery's Handbook, 31st Edition, Ball and Acme Lead Screws.</li>
<li>Engineering Mechanics, Chapter 6/5 – Screws.</li>
<li><a href="https://www.mcmaster.com/99030A993/">McMaster-Carr – Lead Screw</a></li>
<li><a href="https://www.mcmaster.com/95120A592/">McMaster-Carr – Bronze Flange Nut</a></li>
<li><a href="https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48">Grainger – T-Slot Framing</a></li>
</ol>
