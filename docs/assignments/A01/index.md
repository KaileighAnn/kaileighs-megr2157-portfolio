<img width="265" height="439" alt="tong-arms" src="https://github.com/user-attachments/assets/d22b5cfb-77d8-44a4-b17d-53bf5a3ab4ad" />
# A1 – Create Portfolio
## Decide

### Homepage Identity
I chose to make my homepage explain what this portfolio is and what someone can expect to find in it. Since a professor, another engineering student, or even a future employer could be looking through my work, I wanted the organization and purpose to be easy to understand from the beginning. The homepage explains that each assignment will show my analysis, design decisions, calculations, assumptions, and reasoning instead of only showing a final answer. I also kept the assignments organized individually so a reader can quickly find a specific project and follow how I reached my results. My goal is for someone looking through my portfolio to understand both the work I completed and the reasoning behind it without needing me to explain it to them.

### Intentional Customization
For my intentional customization, I changed the assignment labels in the navigation menu to include the name of each assignment instead of only showing the assignment number. For example, “A5” is now labeled “A5 - Bracket Design.” I made this change to make the portfolio easier to navigate, especially for someone who is not familiar with the course or what each assignment number represents. The original labels only showed the assignment numbers, which would require a reader to open each page to know what it contains. Adding the assignment names allows a reader to quickly identify and find a specific project directly from the navigation menu.

### Documentation Standard
For every assignment in this portfolio, I will include my calculations, assumptions, engineering reasoning, and design decisions with enough detail that another engineering student could follow my process and understand how I reached my final result without needing additional explanation.

## Analyze

### Task A - Portfolio Analysis

#### Portfolio 1: Aidan Bradley Engineering Portfolio

**Portfolio:** [Aidan Bradley Engineering Portfolio](https://aocb.github.io/)

**Navigability:** The portfolio separates information into different pages for projects, education, work experience, and contact information. This makes it possible for a reader to move between different types of information without searching through one long page. The projects are also separated by topic, which makes individual work easier to locate. A specific area of the portfolio can be reached in under 60 seconds because the information is divided into recognizable categories.

**Reproducibility:** The portfolio provides descriptions and visual evidence of engineering work, but it does not consistently provide enough technical information for another engineer to fully reproduce each project. More detailed dimensions, calculations, assumptions, materials, and procedures would be needed to recreate the work without asking additional questions.

**Evidence of Reasoning:** The portfolio shows completed engineering projects and provides background about the work, but the reasoning behind individual design decisions is not always documented in detail. Including alternatives that were considered, selection criteria, calculations, and explanations for why specific designs were chosen would provide stronger evidence of the engineering decision-making process.

**Professional Tone:** The portfolio focuses on Bradley's engineering interests, experience, and projects. The language is appropriate for introducing his experience to an employer, although some sections use a more conversational style. The content stays focused on his engineering background and technical interests.


#### Portfolio 2: Rohan Jamal Engineering Portfolio

**Portfolio:** [Rohan Jamal Engineering Portfolio](https://rohanjamal.ca/)

**Navigability:** The homepage provides direct links to individual projects and separates the site into About Me, Projects, Resume, and Contact sections. Each project has a descriptive title, such as "Small-Engine Vehicle Design Project," instead of only using project numbers. This allows a reader to identify the type of work before opening the page and locate a specific project in under 60 seconds.

**Reproducibility:** The project pages provide technical details about how the projects function and how they were developed. For example, the small-engine vehicle page describes the use of a centrifugal clutch, chain transmission, throttle control, and modifications to the original frame. However, another engineer would still need additional information such as dimensions, component specifications, drawings, and calculations to completely reproduce the vehicle.

**Evidence of Reasoning:** The portfolio provides evidence of engineering decision-making. In the small-engine vehicle project, Jamal explains that a centrifugal clutch was selected because it provided a simpler solution than using a separate gearbox and transmission. He also discusses disadvantages of this decision, including lower torque during acceleration and higher engine speed while cruising. Including both the reason for the selection and its tradeoffs helps the reader understand why the design decision was made.

**Professional Tone:** The portfolio uses technical terminology when discussing projects and organizes the engineering work into separate project pages with descriptions, images, and explanations. The homepage is somewhat conversational, while the individual project pages become more technical when explaining components and design decisions. This makes the project documentation appropriate for an engineering or employment audience while still allowing the portfolio to reflect the author's personality.

### Task B - Product Analysis

#### Product: Kitchen Tongs

The product I selected is a pair of metal kitchen tongs. For the purpose of this analysis, the tongs are modeled as three main components: (1) the two metal arms that form the tong body, (2) the spring/pivot mechanism, and (3) the pull/locking ring. These components work together to grip, lift, and release objects.

#### Primary Function

The primary function of the tongs is to convert a force applied by the user's hand into controlled gripping forces at the ends of the two arms. This allows an object, such as food, to be grasped, lifted, rotated, and released while keeping the user's hand a distance away from the object.

#### Governing Model

The primary mechanical behavior of the tongs can be modeled using the moment equation:

**M = Fd**

where:

- **M** = moment about the pivot
- **F** = applied force
- **d** = perpendicular distance from the pivot to the line of action of the force

Each arm can be treated as a lever rotating about the pivot. When a force is applied to the handles, a moment is created about the pivot, causing the gripping ends to move toward each other and apply force to the object.

For a simplified static analysis, the relationship can be written as:

**F_hand × d_hand = F_grip × d_grip**

where:

- **F_hand** = force applied by the user's hand
- **d_hand** = perpendicular distance from the pivot to the hand force
- **F_grip** = force applied to the object at the gripping end
- **d_grip** = perpendicular distance from the pivot to the gripping force

One assumption used in this model is that the two metal arms can be treated as rigid bodies, meaning that deformation of the arms during normal use is small enough to be neglected. Friction at the pivot is also assumed to be small.

#### Components and Geometry

For the purpose of this analysis, the tongs are modeled as three main components.

##### Component 1 - Arms (Tong Body)

<img width="265" height="439" alt="tong-arms" src="https://github.com/user-attachments/assets/c129aa79-e513-423e-a280-ca9c52b18d98" />


The two metal arms form the main body of the tongs. The arms are long and rigid with a formed cross-section that increases stiffness while keeping the weight low. The gripping ends are shaped with slight bends and scallops to increase contact with the object and help prevent it from slipping. The length of the arms also creates distance between the user's hand and the object being handled.

##### Component 2 - Spring/Pivot Mechanism

![Spring and pivot mechanism of kitchen tongs](tong-spring-pivot.jpg)

The spring and pivot mechanism connects the tong body and allows the arms to rotate relative to each other. The coil spring provides a restoring force that pushes the arms apart when the user releases the handles. When the handles are squeezed, energy is stored in the spring. When the hand force is removed, the spring releases that stored energy and returns the tongs toward their open position.

##### Component 3 - Pull/Locking Ring

![Pull and locking ring of kitchen tongs](tong-locking-ring.jpg)

The pull/locking ring allows the tongs to be held in the closed position for storage. Pulling the ring engages the locking mechanism and prevents the spring from opening the arms. Releasing the lock allows the spring mechanism to open the tongs again. The circular shape also provides an easy surface for the user to grip when operating the locking feature.

#### Patent Research

A related patent for this type of tong mechanism is **U.S. Patent US7448660B2, "Tongs with Encapsulated Locking Mechanism."** The listed inventors are **Shunji Yamanaka, Hisato Ogata, and Eugene Kaneko**.

This patent is not being identified as the patent for this exact pair of tongs. Instead, it documents a closely related tong design that uses pivoting arms and a locking mechanism to perform the same primary mechanical function.

**Patent:** [US7448660B2 - Tongs with Encapsu<img width="1552" height="2739" alt="US07448660-20081111-D00003" src="https://github.com/user-attachments/assets/10e3524c-ffd5-403f-ab72-162bcf879b65" />
lated Locking Mechanism](https://patents.google.com/patent/US7448660B2/en)

#### Alternative Solutions

Two alternative devices that perform the same basic mechanical function are:

1. **Spring-style tongs:** The arms can be joined by a single flexible piece of metal that acts as a spring. Elastic deformation of the material allows the arms to return toward their open position when the user releases them.

2. **Scissor-style tongs:** Two crossing members can be connected at a central pivot similar to scissors. Applying force to the handles causes the gripping ends to move toward each other and hold an object.

#### Design Decision

One noticeable design decision in these tongs is the use of long, formed metal arms combined with a spring and locking mechanism. I think the long arms were selected to keep the user's hand farther away from hot food or cooking surfaces while still allowing the user to control the gripping ends. The formed shape of the metal increases the stiffness of the arms without requiring thick or heavy material. The shaped gripping ends provide more contact with the object and help reduce slipping. The spring automatically returns the tongs toward the open position, while the locking ring allows them to remain closed when they are being stored. Together, these design choices create a tool that is lightweight, easy to operate, and able to grip objects while keeping the user's hand away from the working area.

#### Product: Key-Shaped Bottle Opener

The product I selected is a handheld metal bottle opener shaped like a decorative key. The bottle opener is made as one rigid metal component. The decorative features give it the appearance of a key, while the hooked opening near the upper portion of the product provides the geometry needed to remove a bottle cap.

#### Primary Function

The primary mechanical function of the bottle opener is to convert a force applied by the user's hand into a moment that lifts and removes a crown-style bottle cap. The hooked portion of the opener engages underneath the edge of the bottle cap while another contact point rests against the cap. Applying force to the long handle causes the opener to rotate and pry the cap upward.

#### Governing Model

The primary mechanical behavior of the bottle opener can be modeled using the moment equation:

**M = Fd**

where:

- **M** = moment produced about the contact point
- **F** = force applied by the user's hand
- **d** = perpendicular distance from the contact point to the line of action of the applied force

The opener can be modeled as a lever. For a simplified static analysis, the relationship between the input and output forces can be written as:

**F_hand × d_hand = F_cap × d_cap**

where:

- **F_hand** = force applied by the user's hand
- **d_hand** = perpendicular distance from the contact point to the hand force
- **F_cap** = force applied by the opener to the bottle cap
- **d_cap** = perpendicular distance from the contact point to where the opening feature acts on the cap

The long handle creates a larger moment arm than the short distance between the contact point and the edge of the bottle cap. This allows the user to produce the moment needed to remove the cap with a smaller hand force.

One assumption used in this model is that the bottle opener can be treated as a rigid body. Any bending or deformation of the metal during normal use is assumed to be small enough that it does not significantly affect the lever action. Friction and deformation of the bottle cap are also neglected in the simplified model.

#### Component and Geometry

##### Component 1 - Bottle Opener Body

[INSERT PHOTO OF BOTTLE OPENER HERE]

The bottle opener consists of one rigid metal body with a long handle and a hooked opening feature. The length of the handle increases the perpendicular distance between the user's applied force and the contact point at the bottle cap. Since moment is equal to force multiplied by perpendicular distance, this geometry allows the user to create a larger moment with less applied force.

The hooked feature is shaped to fit underneath the edge of a crown-style bottle cap. The nearby metal surface provides another contact point against the cap, creating the lever action needed to rotate and lift the cap. The decorative key-shaped geometry also provides enough length and surface area for the user to hold the opener while applying force.

#### Patent Research

A related historical patent for a lever-style bottle opener is **U.S. Patent US1490149A, "Bottle Opener."** The listed inventor is **Harry L. Vaughan**. The patent was filed in 1921 and published in 1924.

This patent is not being identified as the patent for this exact decorative key-shaped bottle opener. Instead, it documents a related handheld device designed to remove crown-style bottle caps through mechanical leverage.

**Patent:** [US1490149A - Bottle Opener](https://patents.google.com/patent/US1490149A/en)

#### Alternative Solutions

Two alternative devices that perform the same primary mechanical function are:

1. **Wall-mounted bottle opener:** A fixed opener is attached to a wall or other rigid surface. The bottle is moved relative to the opener so that the metal feature engages the underside of the cap and applies the force needed to remove it.

2. **Church-key style bottle opener:** A handheld metal opener uses a short hooked feature and a rigid handle to engage the edge of a bottle cap. The user applies force to the handle to create a moment that pries the cap away from the bottle.

#### Design Decision

One noticeable design decision in this bottle opener is the use of a long handle compared with the small hooked feature that contacts the bottle cap. I think this geometry was selected to increase the distance between the user's applied force and the contact point on the cap. Because the moment produced depends on both force and perpendicular distance, increasing the handle length allows the user to generate the required moment with less hand force.

The hooked opening is also positioned near one end of the product rather than near the center. This leaves most of the product available to act as the handle and increases the available moment arm. The key-shaped design adds a decorative appearance without changing the basic lever mechanism used to remove the cap.
