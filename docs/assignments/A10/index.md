
<h1>A10 – Lead Screw Translating System Design</h1>

<h2>Group Members</h2>

<ul>
<li><strong style="color: #27834A;">Gracie Steelmon</strong> – Calculations and Component Selection</li>
<li><strong style="color: #C64A4A;">Kaileigh Hill</strong> – SolidWorks CAD and Assembly</li>
<li><strong style="color: #3476BA;">Kelsey Skipper</strong> – FEA and Engineering Drawing</li>
</ul>

<hr>

<h2>Project Objective</h2>

<p>
The objective was to design a mechanical tensile tester capable
of applying a 2 kN load using two Acme lead screws and a
moving crosshead.
</p>

<h3>Design Requirements</h3>

<table>
<thead>
<tr><th>Parameter</th><th>Requirement</th></tr>
</thead>
<tbody>
<tr><td>Maximum Load</td><td>2 kN</td></tr>
<tr><td>Crosshead Speed</td><td>1–50 mm/min</td></tr>
<tr><td>Minimum Lead Screw Length</td><td>18 in</td></tr>
<tr><td>Number of Lead Screws</td><td>2</td></tr>
<tr><td>Safety Factor</td><td>4</td></tr>
<tr><td>Maximum Deflection</td><td>0.1 mm</td></tr>
<tr><td>System</td><td>Mechanical, Bench-Top</td></tr>
</tbody>
</table>

<hr>

<!-- GREEN SECTION -->

<div style="background-color: #DDF3E4; color: #243B2B; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h2>1. Lead Screw Diameter Analysis</h2>

<p>
The minimum lead screw diameter was calculated using axial stress
and a safety factor of 4. The 2 kN load was divided equally
between the two screws.
</p>

<p><strong>Load per Screw = 1,000 N</strong></p>

<img width="900" style="max-width:100%; height:auto;" alt="Lead Screw Diameter Calculations" src="https://github.com/user-attachments/assets/0bc8769c-7e0f-414c-87d1-cb67aca92aaa">

<p><em>Figure 1: Minimum lead screw diameter calculations.</em></p>

<hr>

<h2>2. Lead Screw Rotational Speed</h2>

<p>
The rotational speed was calculated using the required
crosshead speed of 1–50 mm/min and the screw lead.
</p>

<p><strong>Rotational Speed = Linear Speed / Screw Lead</strong></p>

<img width="900" style="max-width:100%; height:auto;" alt="Rotational Speed Calculations" src="https://github.com/user-attachments/assets/5793dd42-ea1c-4d6d-a522-5dc81a2d18b7">

<p><em>Figure 2: Lead screw rotational speed calculations.</em></p>

<hr>

<h2>3. Lead Screw Torque and Selection</h2>

<p>
The required torque was calculated using the axial load,
screw geometry, and thread friction.
</p>

<img width="900" style="max-width:100%; height:auto;" alt="Lead Screw Torque Calculations" src="https://github.com/user-attachments/assets/9f676d49-c27e-41a1-a888-4aa0584f988e">

<p><em>Figure 3: Lead screw torque and selection calculations.</em></p>

<h3>Selected Lead Screws</h3>

<table>
<thead>
<tr><th>Feature</th><th>Specification</th></tr>
</thead>
<tbody>
<tr><td>Thread</td><td>3/8"-12 Acme</td></tr>
<tr><td>Direction</td><td>Right-Hand</td></tr>
<tr><td>Material</td><td>Carbon Steel (Grade to Verify)</td></tr>
<tr><td>Length</td><td>3 ft</td></tr>
<tr><td>Quantity</td><td>2</td></tr>
</tbody>
</table>

<p>
<a href="https://www.mcmaster.com/99030A993/" target="_blank">
McMaster-Carr Lead Screw
</a>
</p>

<hr>

<h2>4. Bronze Nut Selection</h2>

<p>
The bronze flange nuts were evaluated using internal thread
bending stress to check their ability to support the applied load.
</p>

<img width="900" style="max-width:100%; height:auto;" alt="Bronze Nut Calculations" src="https://github.com/user-attachments/assets/b9c1b330-5509-4edb-b046-5df9507ad84a">

<p><em>Figure 4: Bronze flange nut calculations.</em></p>

<h3>Selected Nuts</h3>

<table>
<thead>
<tr><th>Feature</th><th>Specification</th></tr>
</thead>
<tbody>
<tr><td>Component</td><td>Acme Bronze Flange Nut</td></tr>
<tr><td>Thread</td><td>3/8"-12 Right-Hand</td></tr>
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

<h2>5. Crosshead Strength Analysis</h2>

<p>
Beam bending stress calculations were used to evaluate the
crosshead under the applied tensile load and safety factor.
</p>

<img width="900" style="max-width:100%; height:auto;" alt="Crosshead Strength Calculations" src="https://github.com/user-attachments/assets/34af6662-71ff-4374-9932-6b10a0f673f6">

<p><em>Figure 5: Crosshead stress and strength calculations.</em></p>

<hr>

<h2>6. Crosshead Deflection Analysis</h2>

<p>
Beam deflection calculations were used to check the
crosshead against the maximum allowable deflection
of 0.1 mm.
</p>

<img width="900" style="max-width:100%; height:auto;" alt="Crosshead Deflection Calculations" src="https://github.com/user-attachments/assets/f723f418-93d1-4be7-bb61-61c2c73579ab">

<p><em>Figure 6: Crosshead deflection calculations.</em></p>

<hr>

<h2>7. Crosshead Multiview Sketch</h2>

<p>
A preliminary sketch was created to show the crosshead
dimensions and lead screw locations before CAD modeling.
</p>

<img width="900" style="max-width:100%; height:auto;" alt="Crosshead Multiview Sketch" src="https://github.com/user-attachments/assets/f49ef004-394b-4722-bd9e-192b35f878ea">

<p><em>Figure 7: Preliminary crosshead multiview sketch.</em></p>

</div>

<hr>

<h2>8. Material Cost Analysis</h2>

<table>
<thead>
<tr>
<th>Component</th>
<th>Quantity</th>
<th>Unit Cost</th>
<th>Total</th>
<th>Link</th>
</tr>
</thead>
<tbody>
<tr>
<td>3/8"-12 Acme Lead Screw</td>
<td>2</td>
<td>$35.32</td>
<td>$70.64</td>
<td><a href="https://www.mcmaster.com/99030A993/">McMaster-Carr</a></td>
</tr>
<tr>
<td>Bronze Flange Nut</td>
<td>2</td>
<td>$111.78</td>
<td>$223.56</td>
<td><a href="https://www.mcmaster.com/95120A592/">McMaster-Carr</a></td>
</tr>
<tr>
<td>T-Slot Framing</td>
<td>1</td>
<td>$245.87</td>
<td>$245.87</td>
<td><a href="https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48">Grainger</a></td>
</tr>
<tr>
<td><strong>Total</strong></td>
<td></td>
<td></td>
<td><strong>$540.07</strong></td>
<td></td>
</tr>
</tbody>
</table>

<p>
The estimated component cost was <strong>$540.07</strong>,
excluding machining and additional hardware.
</p>

<hr>

<!-- RED SECTION -->

<div style="background-color: #FCE3E3; color: #4A2424; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h2>9. SolidWorks CAD and Assembly</h2>

<h3>9.1 Crosshead Modeling</h3>

<p>
The crosshead was modeled in SolidWorks using the dimensions
from the team's calculations. A rectangular profile was
extruded, and two lead screw openings were added using
Extruded Cut.
</p>

<h3>Crosshead Dimensions</h3>

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
<tr><td>Material</td><td>A36 Steel</td></tr>
</tbody>
</table>

<img width="960" style="max-width:100%; height:auto;" alt="Initial Crosshead Model" src="https://github.com/user-attachments/assets/dde21ab3-a162-4c19-b113-25595c0aabb6">

<p><em>Figure 8: Initial SolidWorks crosshead model.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Completed Crosshead Model" src="https://github.com/user-attachments/assets/c9d4eb3e-d79a-4626-9064-69ef4d9a6c7d">

<p><em>Figure 9: Completed crosshead with lead screw openings.</em></p>

<hr>

<h3>9.2 CAD Components</h3>

<p>
Manufacturer CAD files for the lead screws and bronze
flange nuts were downloaded from McMaster-Carr.
The T-slot framing model was obtained from Grainger.
</p>

<img width="960" style="max-width:100%; height:auto;" alt="Bronze Flange Nut" src="https://github.com/user-attachments/assets/67b3ee42-274f-4259-9dd5-ecd0a2453d9f">

<p><em>Figure 10: Bronze Acme flange nut CAD model.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Acme Lead Screw" src="https://github.com/user-attachments/assets/62e8d474-b98e-4cfc-9dce-502b1d3796c5">

<p><em>Figure 11: Acme lead screw CAD model.</em></p>

<hr>

<h3>9.3 Assembly</h3>

<p>
The crosshead was inserted into a SolidWorks assembly.
The bronze flange nuts were positioned underneath the
crosshead using concentric and coincident mates.
</p>

<p>
The two lead screws were aligned with the nuts, and
the T-slot frame was added to complete the assembly.
</p>

<img width="960" style="max-width:100%; height:auto;" alt="Crosshead and Flange Nuts" src="https://github.com/user-attachments/assets/3d28f4ba-af76-4e79-ae5c-d5eaef791a7f">

<p><em>Figure 12: Crosshead with bronze flange nuts.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Lead Screw Assembly" src="https://github.com/user-attachments/assets/d78998ab-44d5-4194-861c-32d321561d8b">

<p><em>Figure 13: Crosshead, lead screws, and flange nuts.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Overall Tensile Tester Assembly" src="https://github.com/user-attachments/assets/f0d4743e-ddaa-48bc-950b-b4cef81cd20d">

<p><em>Figure 14: Completed tensile tester CAD assembly.</em></p>

<hr>

<h3>9.4 CAD Files</h3>

<p>
<a href="https://github.com/user-attachments/files/34669260/Assem2.zip">
<strong>Download SolidWorks CAD Assembly</strong>
</a>
</p>

</div>

<hr>

<!-- BLUE SECTION -->

<div style="background-color: #E8F1FA; color: #243B53; padding: 20px; border-radius: 10px; margin: 20px 0;">

<h2>10. Finite Element Analysis (FEA)</h2>

<h3>10.1 Objective</h3>

<p>
SolidWorks Simulation was used to evaluate crosshead stress,
displacement, and factor of safety under a 2,000 N load.
The required safety factor was 4, with a maximum
vertical deflection of 0.1 mm.
</p>

<h3>10.2 Analyze – Simulation Setup</h3>

<p>
A static simulation was created using a 2,000 N downward
force and fixed supports at the two lead screw/nut
mounting regions.
</p>

<img width="960" style="max-width:100%; height:auto;" alt="FEA Simulation Setup" src="https://github.com/user-attachments/assets/a7412365-4644-4086-9fd5-d6fc9a4bafea">

<p><em>Figure 15: SolidWorks FEA setup.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="FEA Boundary Conditions" src="https://github.com/user-attachments/assets/ef69c8be-1cc0-41e1-97b5-62ab791b058d">

<p><em>Figure 16: Applied force and fixed supports.</em></p>

<h3>10.3 Material and Mesh</h3>

<p>
Material properties were assigned, and a solid mesh was
generated. The mesh was refined to check the consistency
of the results.
</p>

<img width="607" style="max-width:100%; height:auto;" alt="SolidWorks Mesh" src="https://github.com/user-attachments/assets/2daa7e67-f124-4f4f-8052-2feded689d84">

<p><em>Figure 17: SolidWorks simulation mesh.</em></p>

<h3>10.4 FEA Results</h3>

<p>
Von Mises stress, displacement, and factor of safety
were evaluated using SolidWorks Simulation.
</p>

<img width="960" style="max-width:100%; height:auto;" alt="FEA Results" src="https://github.com/user-attachments/assets/a5b6921c-4a2a-4504-be27-3a66ee103463">

<p><em>Figure 18: Crosshead FEA results.</em></p>

<img width="960" style="max-width:100%; height:auto;" alt="Additional FEA Results" src="https://github.com/user-attachments/assets/ae881999-23fa-4953-ad09-853eed2b4715">

<p><em>Figure 19: Additional simulation results.</em></p>

<h3>10.5 Decide – Evaluation</h3>

<p>
The FEA indicated that the selected crosshead design
did not adequately support the 2 kN load.
Further changes to the material or geometry would
be needed to meet the design requirements.
</p>

<hr>

<h2>11. Engineering Drawing</h2>

<h3>11.1 Communicate</h3>

<p>
A multiview SolidWorks engineering drawing was created
with dimensions, tolerances, and a title block following
ASME Y14.5 standards.
</p>

<h3>General Tolerances</h3>

<table>
<thead>
<tr><th>Precision</th><th>Tolerance</th></tr>
</thead>
<tbody>
<tr><td>X.X</td><td>±0.02 in</td></tr>
<tr><td>X.XX</td><td>±0.01 in</td></tr>
<tr><td>X.XXX</td><td>±0.005 in</td></tr>
</tbody>
</table>

<img width="823" style="max-width:100%; height:auto;" alt="Crosshead Engineering Drawing" src="https://github.com/user-attachments/assets/75371664-f118-46c5-852b-8c5e30228bd8">

<p><em>Figure 20: Crosshead engineering drawing.</em></p>

</div>

<hr>

<h2>12. Project Time and Resources</h2>

<table>
<thead>
<tr><th>Task</th><th>Time</th></tr>
</thead>
<tbody>
<tr><td>Calculations and Component Selection</td><td>2 hours</td></tr>
<tr><td>Crosshead CAD and Assembly</td><td>1 hour</td></tr>
<tr><td>FEA and Engineering Drawing</td><td>3 hours</td></tr>
<tr><td>Documentation</td><td>1 hour</td></tr>
<tr><td><strong>Total</strong></td><td><strong>7 hours</strong></td></tr>
</tbody>
</table>

<h3>Resources</h3>

<ul>
<li>SolidWorks and SolidWorks Simulation</li>
<li>McMaster-Carr</li>
<li>Grainger</li>
<li>Machinery's Handbook</li>
<li>Course Materials</li>
</ul>

<hr>

<h2>13. Lessons Learned</h2>

<div style="background-color: #DDF3E4; color: #243B2B; padding: 20px; border-radius: 10px; margin: 20px 0;">

<p>
[INSERT LESSONS LEARNED FROM CALCULATIONS AND COMPONENT SELECTION]
</p>

</div>

<div style="background-color: #FCE3E3; color: #4A2424; padding: 20px; border-radius: 10px; margin: 20px 0;">

<p>
This project helped me understand how component dimensions
affect an assembly. I also gained experience using SolidWorks
mates and manufacturer CAD files to assemble a mechanical system.
</p>

</div>

<div style="background-color: #E8F1FA; color: #243B53; padding: 20px; border-radius: 10px; margin: 20px 0;">

<p>
Through this assignment, I learned how to apply axial loading and boundary conditions
in SolidWorks Simulation to evaluate the structural behavior of a mechanical
component. I also gained experience interpreting stress and displacement results and
understanding how changes in geometry can affect the performance of a design. I also
learned that I should keep using Fusion.
</p>

</div>

<hr>

<h2>14. References</h2>

<ol>
<li>Machinery's Handbook, 31st Edition.</li>
<li>Engineering Mechanics Course Materials.</li>
<li><a href="https://www.mcmaster.com/99030A993/">McMaster-Carr – Acme Lead Screw</a></li>
<li><a href="https://www.mcmaster.com/95120A592/">McMaster-Carr – Bronze Flange Nut</a></li>
<li><a href="https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48">Grainger – T-Slot Framing</a></li>
</ol>



vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv


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

<img width="1796" height="2364" alt="image" src="https://github.com/user-attachments/assets/f49ef004-394b-4722-bd9e-192b35f878ea" />

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

<h3>Objective</h3>

<p>
The objective of my portion of this group assignment was to perform
Finite Element Analysis (FEA) on the tensile tester crosshead using
SolidWorks Simulation. I evaluated the crosshead under a 2,000 N axial
load to determine its stress, displacement, and factor of safety.
</p>

<p>
The design requirements included a minimum factor of safety of
<strong>4</strong> and a maximum vertical deflection of
<strong>0.1 mm</strong>.
</p>

<p>
I was also responsible for creating a detailed engineering drawing
of the crosshead with appropriate dimensions, tolerances, and a
title block.
</p>

<hr>

<h3>10.1 Analyze – Simulation Setup</h3>

<p>
I began by importing the team's tensile tester assembly into
SolidWorks and creating a static simulation study.
</p>

<p>
I applied a <strong>2,000 N downward force</strong> to the
crosshead and selected the two lead screw/nut mounting regions
as fixed supports.
</p>

<img width="960" style="max-width:100%; height:auto;"
alt="SolidWorks FEA Simulation Setup"
src="https://github.com/user-attachments/assets/a7412365-4644-4086-9fd5-d6fc9a4bafea">

<p><em>Figure 15: SolidWorks Simulation setup showing the tensile tester crosshead.</em></p>

<img width="960" style="max-width:100%; height:auto;"
alt="FEA Boundary Conditions"
src="https://github.com/user-attachments/assets/ef69c8be-1cc0-41e1-97b5-62ab791b058d">

<p><em>Figure 16: Applied loading and fixed support locations used for the static analysis.</em></p>

<h3>10.2 Material Properties and Meshing</h3>

<p>
I assigned the selected material properties and generated
a solid mesh to evaluate the crosshead's structural behavior.
</p>

<p>
The mesh divides the crosshead into smaller elements,
allowing SolidWorks Simulation to approximate the
distribution of stress and displacement throughout
the component.
</p>

<img width="607" style="max-width:100%; height:auto;"
alt="SolidWorks FEA Mesh"
src="https://github.com/user-attachments/assets/2daa7e67-f124-4f4f-8052-2feded689d84">

<p><em>Figure 17: Solid mesh generated for the tensile tester crosshead.</em></p>

<h3>10.3 FEA Results</h3>

<p>
I evaluated the maximum von Mises stress, vertical
displacement, and factor of safety to determine whether
the crosshead satisfied the project requirements.
</p>

<p>
I also refined the mesh to check the consistency
of the simulation results.
</p>

<img width="960" style="max-width:100%; height:auto;"
alt="SolidWorks FEA Results"
src="https://github.com/user-attachments/assets/a5b6921c-4a2a-4504-be27-3a66ee103463">

<p><em>Figure 18: SolidWorks Simulation results for the tensile tester crosshead.</em></p>

<img width="960" style="max-width:100%; height:auto;"
alt="Additional FEA Results"
src="https://github.com/user-attachments/assets/ae881999-23fa-4953-ad09-853eed2b4715">

<p><em>Figure 19: Additional FEA results used to evaluate crosshead performance.</em></p>

<h3>10.4 Decide – Design Evaluation</h3>

<p>
Based on the FEA results, I concluded that the selected
crosshead design did not provide sufficient structural
performance under the applied 2 kN load.
</p>

<p>
The simulation demonstrated the importance of evaluating
both material properties and component geometry when
designing a structural member subjected to tensile loading.
</p>

<p>
Further design modifications or material changes would
need to be evaluated to satisfy the required factor
of safety and deflection limits.
</p>

<hr>

<h2>11. MEGR 2157 – Detailed Engineering Drawing – Kelsey Skipper</h2>

<h3>11.1 Communicate – Engineering Drawing</h3>

<p>
I documented the simulation setup, boundary conditions,
and FEA results using screenshots from SolidWorks.
</p>

<p>
I also created a multiview engineering drawing of
the crosshead with dimensions, tolerances, and a
title block following ASME Y14.5 standards.
</p>

<h3>General Tolerance Requirements</h3>

<table>
<thead>
<tr>
<th>Decimal Precision</th>
<th>Tolerance</th>
</tr>
</thead>
<tbody>
<tr><td>X.X</td><td>±0.02 in</td></tr>
<tr><td>X.XX</td><td>±0.01 in</td></tr>
<tr><td>X.XXX</td><td>±0.005 in</td></tr>
</tbody>
</table>

<img width="823" style="max-width:100%; height:auto;"
alt="Crosshead Engineering Drawing"
src="https://github.com/user-attachments/assets/75371664-f118-46c5-852b-8c5e30228bd8">

<p><em>Figure 20: Detailed SolidWorks engineering drawing of the tensile tester crosshead.</em></p>

<hr>

<h3>11.2 Lessons Learned – Kelsey Skipper</h3>

<p>
Through this assignment, I learned how to apply axial
loading and boundary conditions in SolidWorks Simulation
to evaluate the structural behavior of a mechanical
component.
</p>

<p>
I also gained experience interpreting stress and
displacement results and understanding how changes
in geometry can affect the performance of a design.
</p>

<h3>11.3 Time Spent</h3>

<p>
The total time spent on my portion of the assignment
was approximately <strong>3 hours</strong>.
</p>

<p>
Because I had not previously used SolidWorks,
additional time was spent becoming familiar with
the simulation tools and engineering drawing features.
</p>

</div>

