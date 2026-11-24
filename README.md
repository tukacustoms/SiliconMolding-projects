# TUKA CUSTOMS // ENGINEERING LAB
## Silicone Mold Manufacturing & Casting Development

<p align="center">

**ENGINEERING NOTES · MATERIAL SCIENCE · MOLD DESIGN · MANUFACTURING**

`RESEARCH` `PROTOTYPING` `SILICONE CASTING` `DFM`

**Project:** Silicone Mold Development  
**Department:** Engineering & Product Design  
**Status:** Theoretical Study / Pre-Prototype  
**Revision:** 01  
**Origin:** Tuka Customs Engineering Lab

</p>

---

# 00. PROJECT OVERVIEW

## Objective

This project documents the theoretical study and development of a custom silicone mold manufacturing process, starting with the design of a rigid, 3D-printed mold assembly and progressing toward silicone casting, curing and demolding.

The objective is to develop a repeatable manufacturing process that allows me to produce silicone negatives from custom-designed master parts.

Rather than immediately manufacturing a mold through trial and error, I want to understand the physical, mechanical and material principles behind the process before committing to the first prototype.

The main areas of study are:

- Mold architecture and mechanical design.
- Master preparation and positioning.
- Silicone properties and material selection.
- Pouring channels and air evacuation.
- Mold sealing and structural integrity.
- Gravity pouring and bubble prevention.
- Curing behavior and material compatibility.
- Demolding and mechanical extraction.
- Quality inspection and process optimization.

**Development philosophy:** Understand the process, design the equipment, manufacture the prototype, test the results and document every improvement.

---

# 01. UNDERSTANDING THE MANUFACTURING PROCESS

## 1.1 What is a silicone negative mold?

A silicone negative mold is a flexible reproduction of the external geometry of a master component.

The master is the original positive geometry that defines the final shape of the mold cavity.

During manufacturing, liquid silicone is poured around the master. After curing, the silicone solidifies and reproduces the surface details of the master.

Once the master is removed, the resulting silicone cavity can be used to reproduce the original geometry through subsequent casting operations.

The process can be divided into four fundamental stages:

1. Master preparation.
2. Mold assembly and silicone pouring.
3. Silicone curing and master extraction.
4. Mold inspection and preparation for production.

### Basic manufacturing sequence

```text
MASTER COMPONENT
       |
       v
MASTER PREPARATION
       |
       v
RIGID MOLD BOX ASSEMBLY
       |
       v
SILICONE POURING
       |
       v
CURING
       |
       v
OPEN OUTER MOLD HALVES
       |
       v
REMOVE MASTER CARRIER
       |
       v
SEPARATE MASTER FROM SILICONE
       |
       v
SILICONE NEGATIVE READY
```

## 1.2 Positive and negative geometry

Understanding the relationship between positive and negative geometry is essential.

- **Positive:** The original master component.
- **Negative:** The cavity formed by the cured silicone.
- **Casting:** The material subsequently introduced into the silicone cavity to reproduce the positive geometry.

The quality of the final reproduction depends heavily on the accuracy of the original master, its surface condition, the silicone material and the casting process.

A silicone mold can reproduce very small surface details, but it will also reproduce imperfections, scratches and unwanted features present on the master.

For this reason, master preparation is an important part of mold manufacturing.

---

# 02. MOLD ARCHITECTURE AND MECHANICAL DESIGN

## 2.1 Rigid mold box

The rigid mold box acts as the external structure that contains the liquid silicone during pouring and curing.

Its main functions are:

- Maintain the master in the correct position.
- Contain the liquid silicone.
- Define the external dimensions of the silicone block.
- Prevent deformation during pouring.
- Provide mechanical access for assembly and disassembly.
- Support the pouring and venting systems.

For this project, I am developing a custom mold box using 3D-printed components.

This approach allows me to manufacture complex geometries, experiment with different configurations and modify the design without requiring conventional machining.

## 2.2 Three-piece mold architecture

The current design uses three main mechanical components:

| Component | Function |
|---|---|
| Left outer half | Contains and supports the silicone during curing |
| Right outer half | Completes the mold enclosure |
| Central insert | Holds the master component in position |

The central insert is designed to be removable.

Instead of trying to extract the master while the outer mold halves are still assembled, the system allows the outer halves to open first.

This provides additional mechanical access and reduces the possibility of damaging the silicone during extraction.

### Intended extraction sequence

```text
       ASSEMBLED MOLD
             |
             v
    SILICONE FULLY CURED
             |
             v
    RELEASE OUTER CLAMPS
             |
             v
    SEPARATE OUTER HALVES
             |
             v
    REMOVE CENTRAL INSERT
      + MASTER TOGETHER
             |
             v
    SEPARATE MASTER FROM
       SILICONE NEGATIVE
             |
             v
       FINISHED MOLD
```

## 2.3 Central insert design

The central insert is one of the most important components of this architecture.

It provides a positioning interface for the master and allows the master to be removed together with the insert.

The insert must have:

- A controlled extraction direction.
- Sufficient structural rigidity.
- Accurate positioning relative to the outer mold halves.
- A secure master mounting interface.
- Adequate clearance from surrounding geometry.
- No unwanted mechanical locking features.

### Draft angles

Draft angles are intentional inclinations applied to surfaces to facilitate extraction.

Without draft, surfaces that are nominally parallel to the extraction direction can experience considerable friction, especially when the printed components are not perfectly smooth.

For initial design studies, a draft angle of approximately 2–3° can be considered on non-functional insert surfaces.

This is a preliminary design recommendation, not a universal requirement.

The actual angle depends on the geometry, material, surface finish and extraction direction.

**Important:** Draft angles do not automatically solve undercuts. Any reverse-facing geometry must be evaluated independently.

## 2.4 Alignment and positioning

The outer mold halves and central insert must return to the same position during every assembly.

Misalignment can cause:

- Uneven silicone thickness.
- Incorrect master positioning.
- Silicone leakage.
- Flash formation.
- Uneven contact between mechanical components.

Possible positioning solutions include:

- Dowel pins.
- Cylindrical locating features.
- Male/female registration keys.
- Recessed alignment pockets.

For the first prototype, I intend to investigate two to four locating features depending on the available space.

## 2.5 Clamping system

The clamping system maintains the mold assembly in its intended configuration during pouring and curing.

It must resist the hydrostatic pressure generated by the liquid silicone and prevent the components from separating.

For a simple static mold, the pressure at a depth can be approximated by:

\[
P=\rho gh
\]

Where:

- \(P\) = hydrostatic pressure (Pa).
- \(\rho\) = silicone density (kg/m³).
- \(g\) = gravitational acceleration (m/s²).
- \(h\) = liquid height (m).

Although the pressure in a small mold is generally modest, the assembly still needs to be sufficiently rigid to prevent leakage and deformation.

Possible clamping solutions:

- M3/M4 fasteners.
- External mechanical clamps.
- Threaded inserts.
- Integrated clamping features.

The selected system must allow repeated assembly without damaging the printed components.

---

# 03. MASTER PREPARATION AND SURFACE QUALITY

## 3.1 Master surface preparation

The master defines the final internal geometry of the silicone mold.

Consequently, its surface finish directly influences the quality of the silicone negative.

Before pouring, the master should be inspected for:

- Surface imperfections.
- Layer lines from 3D printing.
- Unwanted holes or cavities.
- Sharp edges.
- Undercuts.
- Contamination.
- Moisture or residues.

Depending on the intended reproduction quality, the master may require sanding, polishing, sealing or surface treatment.

## 3.2 Release agents

A release agent can help prevent silicone from bonding to the master.

However, compatibility must be verified before use.

Some release agents can interfere with silicone curing or contaminate the mold surface.

The selected product must be compatible with the specific silicone chemistry.

The master material must also be considered because certain silicones, particularly some addition-cure formulations, can be inhibited by contaminants or incompatible materials.

A small compatibility test is recommended before manufacturing the complete mold.

## 3.3 Undercuts

Undercuts are geometric features that prevent a rigid component from being extracted along a simple straight direction.

They are particularly important when designing the central insert.

The master and the cured silicone may be flexible relative to one another, but that does not mean every undercut can be safely released.

Excessive deformation can cause:

- Tearing.
- Permanent deformation.
- Surface damage.
- Premature mold failure.

The extraction path must be evaluated in CAD before manufacturing.

---

# 04. SILICONE MATERIAL PROPERTIES

## 4.1 Silicone rubber

Silicone rubber is an elastomeric material known for its flexibility, elastic recovery, thermal stability and resistance to environmental degradation.

Its mechanical properties make it suitable for flexible molds that need to reproduce complex geometries.

However, different silicone formulations can behave very differently.

Material selection must be based on the intended application.

## 4.2 Shore hardness

Shore hardness is a measurement of a material's resistance to indentation.

For silicone rubber, Shore A is commonly used.

| Hardness | General behavior |
|---|---|
| Shore A 10–15 | Very soft and flexible |
| Shore A 20–30 | Medium flexibility |
| Shore A 40–50 | Firmer and more resistant to deformation |
| Shore A 60+ | Relatively rigid elastomer |

These are general descriptions rather than strict material classifications.

A softer silicone can facilitate the removal of masters with complex geometry.

However, very soft silicone may deform more easily during handling and casting.

A harder silicone can provide better dimensional stability but may make extraction more difficult.

The correct hardness must be selected according to:

- Master geometry.
- Undercut complexity.
- Required dimensional accuracy.
- Intended casting material.
- Expected number of production cycles.

## 4.3 Pot life and curing time

Two important parameters must be understood before pouring.

**Pot life:** The amount of time the mixed silicone remains sufficiently workable before its viscosity increases significantly.

**Curing time:** The time required for the silicone to reach the specified cured state.

These values are not interchangeable.

The pouring operation must be completed within the manufacturer's specified working time.

Curing time depends on the formulation, temperature, mixing conditions and other manufacturer-defined parameters.

Always consult the technical datasheet of the selected silicone.

## 4.4 Mixing ratio

Many two-component silicone systems require mixing a base component with a curing agent.

The ratio must be followed precisely.

For example, if the manufacturer specifies a 1:1 mass ratio:

\[
m_A=m_B
\]

Where:

- \(m_A\) = mass of component A.
- \(m_B\) = mass of component B.

For other formulations, the specified ratio may be different.

The ratio must never be assumed.

Incorrect mixing can result in:

- Incomplete curing.
- Soft or sticky regions.
- Poor mechanical properties.
- Reduced mold durability.

A precision scale is recommended for weighing the components.

---

# 05. MOLD VOLUME AND SILICONE CONSUMPTION

## 5.1 Estimating the required silicone quantity

Before pouring, I need to estimate the volume of the mold enclosure and subtract the volume occupied by the master and other solid components.

The theoretical silicone volume can be represented as:

\[
V_s=V_b-V_m-V_i
\]

Where:

- \(V_s\) = required silicone volume.
- \(V_b\) = internal mold box volume.
- \(V_m\) = master volume.
- \(V_i\) = volume occupied by other internal inserts.

This is a simplified approximation.

In practice, I should also account for the pouring funnel, channels, vents and an additional allowance for material loss.

If the mold geometry is complex, the volume can be calculated directly in CAD using the solid bodies.

## 5.2 Converting volume into mass

Once the silicone volume is known, the approximate mass can be calculated using density:

\[
m=\rho V
\]

Where:

- \(m\) = required silicone mass.
- \(\rho\) = silicone density.
- \(V\) = calculated volume.

The density must come from the manufacturer's datasheet.

This calculation helps prevent mixing too little silicone or unnecessarily wasting material.

---

# 06. POURING CHANNELS AND GATE DESIGN

## 6.1 What is a pouring channel?

The pouring channel, also called the gate or sprue depending on its geometry and function, is the passage through which liquid silicone enters the mold enclosure.

Its purpose is to provide a controlled path from the pouring opening into the mold cavity.

The geometry should allow the silicone to enter without excessive restriction.

Important design parameters include:

- Channel diameter.
- Channel length.
- Entrance geometry.
- Funnel shape.
- Cavity orientation.
- Silicone viscosity.
- Pouring speed.

## 6.2 Funnel design

A funnel makes pouring easier and reduces spillage.

The upper opening should be larger than the internal channel.

This provides a larger target for manual pouring and creates a transition into the narrower inlet.

For the first prototype, the following dimensions are proposed:

| Feature | Initial design value |
|---|---:|
| Funnel opening | Ø15 mm |
| Main inlet throat | Ø8 mm |
| Funnel transition | Approximately 45° |

These are experimental starting dimensions for a small-to-medium mold, not validated universal values.

The correct dimensions depend on the silicone viscosity, cavity volume and filling behavior.

## 6.3 Top inlet versus bottom inlet

Two possible configurations were considered.

### Top pouring

The silicone enters through an upper opening and travels through the cavity.

Advantages:

- Simple mold construction.
- Easy access for manual pouring.
- Convenient funnel integration.
- Suitable for gravity-fed filling when the geometry allows proper air evacuation.

Potential limitations:

- Silicone may flow over recessed regions.
- Air can become trapped beneath overhanging features.
- Direct pouring can introduce additional bubbles.

### Bottom pouring

The silicone enters from a lower opening and rises through the cavity.

Advantages:

- Can provide a rising fill front.
- May allow air to move upward toward upper vents.
- Can be useful for complex cavities where bottom filling produces a more controlled filling pattern.

Potential limitations:

- More complicated channel arrangement.
- Requires careful vent placement.
- May require a more controlled pouring setup.

### Current design decision

For the first prototype, I intend to retain the top inlet already integrated into my CAD model.

There is no universal rule stating that a bottom inlet is always better.

The actual performance depends on the cavity geometry and the orientation of the mold during filling.

The most important objective is to prevent air from becoming trapped in regions that are filled early.

The first casting test will help determine whether the current configuration needs modification.

---

# 07. AIR VENTING AND BUBBLE PREVENTION

## 7.1 Why are air vents necessary?

When liquid silicone enters a closed mold enclosure, the air originally occupying the cavity must escape.

If there is no adequate escape path, air can become trapped inside the silicone.

These trapped air pockets can create voids and incomplete surface reproduction.

Air vents provide a path for displaced air to leave the mold.

They are particularly important around:

- Recessed geometry.
- Narrow channels.
- Deep pockets.
- Upper corners.
- Local high points.
- Areas with restricted silicone flow.

## 7.2 Vent positioning

Vent positioning should be based on the actual orientation of the mold during pouring.

The vents should connect the cavity regions most likely to trap air to the exterior.

A vent placed in the wrong location may provide very little benefit.

For gravity pouring, the ideal arrangement generally allows the filling front to displace air toward the vent outlets.

The position of the final air pockets must be evaluated using the geometry and filling orientation.

## 7.3 Vent dimensions

For the first prototype, I am considering the following starting values:

| Feature | Preliminary dimension |
|---|---:|
| Main vent channel | Ø1.0–1.5 mm |
| Larger vent option | Ø2.0 mm |
| External vent outlet | Approximately Ø2 mm |

These dimensions are initial experimental values.

Vent sizing depends on the silicone viscosity, cavity geometry, vent length and pouring speed.

Smaller vents can restrict air movement, while excessively large vents can allow silicone to escape and produce unnecessary flash.

## 7.4 Vent channels versus vent holes

A vent does not necessarily need to be a cylindrical hole extending through the entire mold.

It can be a small channel connecting an air-trapping region to the external environment.

Possible configurations include:

- Straight cylindrical vents.
- Shallow rectangular channels.
- Small grooves along the parting surface.
- Multiple microvents connected to an external outlet.

The design must ensure that the vent remains open during pouring.

## 7.5 Why more vents are not always better

Adding more vents can improve air evacuation, but it also increases the number of potential leakage paths.

The objective is not to maximize the number of vents.

It is to provide sufficient air evacuation at the correct locations.

For the first prototype, I intend to begin with one main vent and add secondary vents only when the geometry or test results justify them.

---

# 08. GRAVITY POURING PROCEDURE

## 8.1 Understanding gravity pouring

Gravity pouring is a process in which liquid silicone enters the mold through an opening under the influence of gravity.

Unlike pressure injection, the material is not forced into the cavity using an external injection system.

The flow depends on:

- Material viscosity.
- Gravity.
- Channel geometry.
- Pouring height.
- Channel restrictions.
- Mold orientation.

The objective is to achieve a continuous filling process while minimizing the introduction of air.

## 8.2 Recommended pouring procedure

The following procedure will be used as the initial experimental workflow.

### Stage 1 — Mold preparation

1. Inspect all printed components.
2. Remove debris and printing residues.
3. Check the alignment features.
4. Verify that the mold halves fit correctly.
5. Inspect the sealing surfaces.
6. Apply a compatible release agent if required.
7. Confirm that the master is securely attached to the central insert.

### Stage 2 — Mold assembly

1. Position the central insert.
2. Install the two outer mold halves.
3. Engage the alignment features.
4. Tighten the clamping system evenly.
5. Verify that no visible gaps remain.
6. Confirm that the pouring inlet and vents are unobstructed.

### Stage 3 — Silicone preparation

1. Read the manufacturer's technical datasheet.
2. Verify the required mixing ratio.
3. Measure the components using an appropriate scale.
4. Mix slowly and thoroughly.
5. Avoid introducing unnecessary air during mixing.

The mixing process must be completed within the available pot life.

### Stage 4 — Pouring

1. Position the mold in the intended pouring orientation.
2. Introduce silicone through the pouring funnel.
3. Maintain a slow and continuous flow.
4. Avoid sudden interruptions or splashing.
5. Observe the vent outlets.
6. Continue until the cavity is completely filled.

The silicone should be introduced in a way that allows the filling front to displace air rather than isolate it inside the cavity.

### Stage 5 — Curing

1. Keep the mold stationary.
2. Avoid disturbing the assembly.
3. Maintain the environmental conditions recommended by the manufacturer.
4. Allow the silicone to cure for the specified period.

The mold should not be opened prematurely.

---

# 09. VACUUM DEGASSING

## 9.1 What is degassing?

Degassing is the removal of entrained air from a liquid material.

During silicone mixing, air can become incorporated into the material.

These bubbles may remain inside the cured silicone and affect the final mold quality.

Vacuum degassing reduces the pressure surrounding the silicone, allowing trapped gas bubbles to expand and escape.

## 9.2 Why it matters

Degassing can help reduce:

- Internal voids.
- Surface imperfections.
- Bubble-related defects.
- Incomplete reproduction of small details.

However, vacuum degassing and mold venting solve different problems.

**Vacuum degassing:** Removes air already incorporated into the mixed silicone.

**Mold venting:** Allows air inside the mold cavity to escape during filling.

One does not replace the other.

## 9.3 Important considerations

When vacuum is applied, the silicone may expand significantly as bubbles grow.

Therefore:

- The mixing container must have sufficient free volume.
- The vacuum chamber must accommodate expansion.
- The silicone must be monitored during degassing.
- The manufacturer's processing recommendations must be followed.

If no vacuum chamber is available, controlled mixing and pouring become even more important.

A vacuum chamber is a useful improvement for future process development, but the first prototype can also be used to evaluate the baseline process without vacuum.

---

# 10. DEMOLDING AND MECHANICAL EXTRACTION

## 10.1 Extraction strategy

The current mold architecture uses a removable central insert carrying the master component.

The extraction sequence is intentionally designed to separate the outer mold halves before removing the central insert.

This provides more clearance and reduces the possibility of mechanical interference.

## 10.2 Extraction forces

When components are separated, the required extraction force may come from several sources:

- Friction between contacting surfaces.
- Adhesion between materials.
- Elastic deformation of silicone.
- Mechanical interference.
- Geometric undercuts.
- Surface roughness.

The extraction system should distribute force across the carrier rather than concentrating it at one point.

## 10.3 Push holes and extraction points

I considered two possible extraction configurations:

**Single larger push hole**

A single push point can be sufficient for a small, rigid and well-supported carrier.

However, applying force away from its center of resistance can cause rotation or tilting.

**Multiple smaller push holes**

Multiple push points can distribute force and reduce the possibility of tilting.

For the current design, I intend to investigate two symmetrical extraction points.

### Preliminary extraction dimensions

| Feature | Initial value |
|---|---:|
| Number of push points | 2 |
| Threaded extraction interface | M5 |
| Possible push-pin diameter | Ø4.8 mm |
| Edge chamfer | 0.5 mm |

These values are preliminary and must be checked against the printed wall thickness and carrier geometry.

A useful solution is to use two threaded M5 jack screws in the outer mold structure.

After opening the outer halves, the screws can be tightened gradually and alternately to push the carrier out.

The screws must contact reinforced pads on the carrier.

They must not push directly against the master or delicate features.

The extraction system must also have sufficient thread engagement and structural support to avoid damaging the printed parts.

## 10.4 Preventing mechanical locking

A major concern is the possibility of silicone entering unintended spaces around the central insert.

If liquid silicone flows behind the insert and cures there, it can create an additional mechanical connection.

This can make extraction difficult or impossible without damaging the mold.

To prevent this, I need to evaluate:

- Contact between the central insert and outer halves.
- Sealing around the insert perimeter.
- Possible leakage paths.
- Reverse-facing surfaces.
- Undercuts.
- Extraction clearance.

The interface must be designed to prevent silicone from entering regions that are not intended to become part of the silicone negative.

---

# 11. 3D PRINTING AND MANUFACTURING CONSIDERATIONS

## 11.1 Why 3D printing?

3D printing allows the production of custom mold components with relatively low manufacturing cost and short iteration cycles.

It is particularly useful for developing:

- Complex internal geometry.
- Custom positioning systems.
- Pouring funnels.
- Vent channels.
- Mechanical extraction features.
- Alignment structures.

However, printed components are not automatically liquid-tight.

## 11.2 Surface finish and sealing

FDM printing can produce layer lines and small gaps between adjacent extrusion paths.

These defects can allow liquid silicone to leak through the mold box.

Potential solutions include:

- Increasing the number of wall perimeters.
- Increasing the number of top and bottom layers.
- Using an appropriate infill strategy.
- Improving dimensional accuracy.
- Applying a compatible surface sealant.
- Testing the assembly before introducing silicone.

The selected printing parameters must also consider the mechanical loads applied during clamping and extraction.

## 11.3 Structural considerations

Particular attention should be given to:

- Thin walls around the cavity.
- Threaded mounting areas.
- Extraction holes.
- Alignment pin supports.
- Clamping interfaces.
- Funnel connections.

The printed components should resist deformation during assembly and handling.

A component that is sufficiently strong under normal handling may still fail when extraction screws apply concentrated forces.

---

# 12. COMMON DEFECTS AND FAILURE MODES

Understanding possible defects before the first prototype helps establish a more effective inspection process.

| Defect | Possible cause | Potential solution |
|---|---|---|
| Air pockets | Insufficient venting | Add or reposition vents |
| Surface bubbles | Air introduced during mixing | Improve mixing or degas |
| Incomplete filling | Restricted flow | Review inlet geometry |
| Silicone leakage | Poor sealing | Improve interfaces |
| Incomplete curing | Incorrect mixing or inhibition | Verify ratio and compatibility |
| Master trapped | Undercuts or mechanical locking | Modify extraction geometry |
| Silicone tearing | Excessive demolding force | Improve release strategy |
| Mold deformation | Insufficient support | Increase structural rigidity |
| Excessive flash | Gaps between components | Improve fit and clamping |
| Dimensional inaccuracies | Master positioning or deformation | Improve alignment and support |

A failed prototype is not necessarily a failed development process.

Each defect should be documented, analyzed and connected to a specific design or process variable.

---

# 13. INITIAL DESIGN SPECIFICATIONS

The following table consolidates the dimensions currently being considered for the first prototype.

**These are starting values for experimentation, not validated production specifications.**

| Parameter | Initial value |
|---|---:|
| Main pouring funnel | Ø15 mm |
| Main pouring inlet | Ø8 mm |
| Primary vent | Ø1–1.5 mm |
| Larger vent option | Ø2 mm |
| Extraction points | 2 |
| Extraction interface | M5 |
| Push-pin diameter | Approximately Ø4.8 mm |
| Insert draft | 2–3° |
| Funnel transition | Approximately 45° |

The final dimensions will depend on the silicone selected, mold geometry, manufacturing tolerances and results of the first casting test.

---

# 14. EXPERIMENTAL DEVELOPMENT PLAN

The first prototype should be treated as an experimental validation stage.

Rather than changing several design parameters simultaneously, I intend to evaluate the system progressively.

## Phase 01 — CAD validation

- [ ] Verify the three-piece mold architecture.
- [ ] Check the master positioning.
- [ ] Verify the central insert extraction direction.
- [ ] Inspect potential undercuts.
- [ ] Check wall thickness.
- [ ] Verify pouring channel continuity.
- [ ] Identify potential air-trapping locations.
- [ ] Inspect sealing interfaces.
- [ ] Verify extraction screw positioning.

## Phase 02 — Printed prototype

- [ ] Manufacture the mold box.
- [ ] Inspect dimensional accuracy.
- [ ] Check alignment pins.
- [ ] Test clamping.
- [ ] Verify that the mold opens correctly.
- [ ] Test central insert extraction without silicone.
- [ ] Check for mechanical interference.
- [ ] Perform a leak test using a suitable non-reactive test fluid if appropriate for the materials and geometry.

## Phase 03 — Silicone preparation

- [ ] Select the silicone formulation.
- [ ] Read the technical datasheet.
- [ ] Confirm the mixing ratio.
- [ ] Verify material compatibility.
- [ ] Estimate silicone volume.
- [ ] Prepare the required tools.
- [ ] Determine whether vacuum degassing is available.
- [ ] Establish the pouring orientation.

## Phase 04 — First casting test

- [ ] Prepare the master.
- [ ] Apply compatible release agent if required.
- [ ] Assemble the mold.
- [ ] Verify sealing.
- [ ] Mix the silicone.
- [ ] Pour at a controlled rate.
- [ ] Observe the vent outlets.
- [ ] Allow the silicone to cure.
- [ ] Open the outer mold halves.
- [ ] Extract the central insert.
- [ ] Remove the master carefully.

## Phase 05 — Inspection and evaluation

- [ ] Inspect the silicone surface.
- [ ] Identify trapped air pockets.
- [ ] Check dimensional reproduction.
- [ ] Inspect the vent locations.
- [ ] Check for flash.
- [ ] Evaluate mold flexibility.
- [ ] Evaluate demolding difficulty.
- [ ] Document extraction problems.
- [ ] Record silicone consumption.
- [ ] Identify improvements for Revision 02.

---

# 15. VARIABLES TO RECORD DURING TESTING

For the first casting, I want to record the actual manufacturing parameters rather than relying only on visual impressions.

| Variable | Recorded information |
|---|---|
| Silicone brand | Manufacturer and product |
| Silicone hardness | Shore A |
| Mixing ratio | Manufacturer specification |
| Mixed silicone mass | Grams |
| Room temperature | °C |
| Pot life | Manufacturer specification / observed |
| Curing time | Hours |
| Vacuum degassing | Yes / No |
| Pouring orientation | Top / Bottom / Other |
| Inlet diameter | mm |
| Vent diameter | mm |
| Number of vents | Quantity |
| Casting result | Pass / Fail |
| Defects | Description |
| Extraction result | Easy / Moderate / Difficult |

These records will help identify relationships between process variables and final mold quality.

---

# 16. ENGINEERING PRINCIPLES TO UNDERSTAND BEFORE PRODUCTION

Before proceeding to a complete manufacturing cycle, I need to understand the following concepts in greater depth.

### Fluid mechanics

- Hydrostatic pressure.
- Viscosity.
- Laminar and turbulent flow.
- Flow restrictions.
- Gravity-driven filling.
- Air displacement.

### Materials science

- Elastomer behavior.
- Shore hardness.
- Elastic recovery.
- Polymer crosslinking.
- Addition-cure versus condensation-cure silicone.
- Chemical compatibility.
- Curing inhibition.

### Mechanical design

- Draft angles.
- Undercuts.
- Parting lines.
- Tolerances and clearances.
- Mechanical alignment.
- Contact pressure.
- Extraction forces.

### Manufacturing engineering

- Design for Manufacturing (DFM).
- Additive manufacturing.
- Surface finishing.
- Dimensional inspection.
- Process repeatability.
- Quality control.

Understanding these subjects will make it possible to move beyond simply following a mold-making tutorial and start designing a manufacturing process based on engineering principles.

---

# 17. FUTURE DEVELOPMENT

After validating the first silicone mold, possible improvements include:

- Optimizing the pouring funnel.
- Testing alternative vent configurations.
- Evaluating vacuum degassing.
- Improving the central insert.
- Reducing silicone consumption.
- Improving extraction mechanics.
- Testing different Shore hardness formulations.
- Improving mold dimensional accuracy.
- Evaluating casting materials and production cycles.

The long-term objective is to establish a repeatable, documented and scalable mold manufacturing workflow for custom Tuka Customs components.

---

# 18. REFERENCES AND TECHNICAL RESEARCH

The theoretical development of this project should be supported by technical documentation and reliable engineering references.

The following sources are recommended for further study:

1. **Silicone manufacturer technical datasheets** — Mixing ratios, viscosity, pot life, curing time, hardness and material compatibility.
2. **Silicone manufacturer processing guides** — Mixing, vacuum degassing, pouring and demolding.
3. **ASTM D2240** — Standard Test Method for Rubber Property: Durometer Hardness.
4. **Engineering Fluid Mechanics textbooks** — Hydrostatic pressure, viscosity and fluid flow.
5. **Polymer Science and Engineering references** — Elastomer chemistry, curing and crosslinking.
6. **Additive Manufacturing references** — FDM printing, dimensional tolerances and surface quality.

Specific product datasheets and experimental observations should be added here once the silicone formulation and manufacturing materials have been selected.

---

# 19. DEVELOPMENT LOG

| Revision | Development stage | Status |
|---|---|---|
| 01 | Theoretical study and initial mold architecture | In progress |
| 02 | CAD validation and mechanical improvements | Pending |
| 03 | First printed mold prototype | Pending |
| 04 | First silicone casting | Pending |
| 05 | Inspection and design corrections | Pending |
| 06 | Validated manufacturing procedure | Pending |

---

<p align="center">

**TUKA CUSTOMS™**

*Engineering through experimentation.*

`DESIGN` · `PROTOTYPE` · `TEST` · `IMPROVE`

**END OF DOCUMENT // REV. 01**

</p>
