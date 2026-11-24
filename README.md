# TUKA CUSTOMS // ENGINEERING LAB
## Silicone Mold Manufacturing & Syringe Injection Development

<p align="center">

**ENGINEERING NOTES · MATERIAL SCIENCE · MOLD DESIGN · ADDITIVE MANUFACTURING**

`SHORE A 55` `SYRINGE FILLING` `MOLD ENGINEERING` `PROTOTYPING`

**Project:** Custom Silicone Mold Development  
**Department:** Engineering & Product Design  
**Revision:** 02  
**Status:** Theoretical Study / Pre-Prototype

</p>

---

# 00. PROJECT OBJECTIVE

The objective of this project is to design and manufacture a custom rigid mold assembly capable of producing silicone negatives from custom-designed master components.

The mold will be manufactured using 3D printing and will incorporate a custom mechanical assembly, a removable central insert, a syringe-based filling system and dedicated air evacuation channels.

The selected target silicone hardness is Shore A 55.

Unlike conventional gravity pouring, this project will use a manual syringe to introduce the uncured silicone into the mold cavity.

This changes several important design considerations, particularly:

- Injection channel geometry.
- Flow resistance.
- Air evacuation.
- Mold sealing.
- Structural rigidity.
- Pressure distribution.
- Material viscosity.
- Filling time and curing time.
- Mechanical extraction.

The intention is to understand the theoretical principles behind each component before manufacturing the first prototype.

**Development approach:** Research → CAD Design → Manufacturing → Assembly → Silicone Filling → Curing → Inspection → Optimization.

---

# 01. UNDERSTANDING THE SILICONE MATERIAL

## 1.1 Shore hardness

Shore hardness is a measurement of a material's resistance to indentation.

For elastomeric materials, Shore A is commonly used to describe the hardness of flexible rubber and silicone.

The selected target for this project is:

**Shore A 55**

This represents a relatively firm elastomer compared with softer silicone formulations.

Its mechanical behavior is important because it directly influences the performance of the finished silicone mold.

Relevant properties include:

| Property | Importance |
|---|---|
| Shore hardness | Resistance to indentation and deformation |
| Tensile strength | Resistance to tensile loading |
| Tear strength | Resistance to tearing during extraction |
| Elongation at break | Ability to stretch before rupture |
| Elastic recovery | Ability to return to its original geometry |
| Viscosity | Resistance to flow before curing |
| Shrinkage | Dimensional changes during curing |

A Shore A 55 silicone may provide a useful balance between dimensional stability and flexibility.

However, hardness alone does not determine whether a silicone is suitable for the intended mold geometry.

Tear strength and elongation are particularly important when extracting masters with undercuts or complex surfaces.

## 1.2 Important distinction: hardness versus viscosity

One of the most important material considerations is understanding that Shore hardness and viscosity describe different properties.

**Shore hardness** describes the mechanical resistance of the cured material.

**Viscosity** describes the resistance of the uncured liquid material to flow.

A silicone with Shore A 55 can have different uncured viscosities depending on its chemical formulation.

This is particularly important because the project uses syringe-based filling.

Before selecting the final silicone, I need to obtain its technical datasheet and verify:

- Uncured viscosity.
- Mixing ratio.
- Pot life.
- Curing time.
- Shore hardness.
- Tensile strength.
- Tear strength.
- Elongation at break.
- Linear shrinkage, if specified.
- Compatibility with the master and mold materials.

The selected silicone must be suitable for the intended syringe-filling method.

---

# 02. MOLD ARCHITECTURE

## 2.1 Rigid printed mold enclosure

The external mold structure will be manufactured using 3D printing.

Its primary function is to contain the liquid silicone and maintain the correct position of the master during filling and curing.

The rigid structure must provide:

- Dimensional stability.
- Accurate alignment.
- Adequate sealing.
- Structural support.
- Access to the injection port.
- Access to the air vents.
- A controlled extraction mechanism.

The enclosure is designed around a three-piece architecture.

## 2.2 Three-piece assembly

The current mechanical design consists of:

| Component | Function |
|---|---|
| Left outer half | Supports and contains the silicone |
| Right outer half | Completes the mold enclosure |
| Central insert | Holds the master component |

The central insert is removable and carries the master during the initial extraction stage.

The outer halves are opened first, providing access to the central insert.

This arrangement is intended to simplify demolding and reduce mechanical interference.

### Assembly and extraction sequence

```text
       MOLD ASSEMBLY
             |
             v
      SYRINGE FILLING
             |
             v
      SILICONE CURING
             |
             v
      OPEN OUTER HALVES
             |
             v
      REMOVE CENTRAL INSERT
        WITH THE MASTER
             |
             v
       SEPARATE MASTER
        FROM SILICONE
             |
             v
       FINISHED NEGATIVE
```

## 2.3 Central insert

The central insert is responsible for maintaining the master in its intended position.

Its geometry must allow extraction without creating mechanical locks.

Important design considerations:

- Controlled extraction direction.
- Adequate wall thickness.
- Structural rigidity.
- Secure master mounting.
- Correct alignment with outer halves.
- Clearance around extraction surfaces.
- No unintended silicone leakage paths.

### Draft angles

Draft angles are inclined surfaces designed to facilitate component extraction.

For preliminary CAD development, approximately 2–3° can be considered on suitable non-functional surfaces.

The final value depends on the extraction direction, surface finish and geometry.

Draft angles do not eliminate the need to inspect undercuts.

## 2.4 Mechanical alignment

The assembly must return to its original position after every disassembly.

Misalignment can produce uneven silicone thickness, incorrect master positioning and leakage.

Possible alignment solutions include:

- Dowel pins.
- Cylindrical locating features.
- Male/female registration keys.
- Recessed alignment pockets.

The number and position of locating features should be determined according to the available geometry.

## 2.5 Custom clamping system

The project uses a custom clamping mechanism rather than assuming a conventional bolted mold enclosure.

The clamping system must maintain contact between the mold components during syringe filling and curing.

Its main engineering requirements are:

- Consistent positioning.
- Resistance to separation.
- Resistance to deformation.
- Uniform contact pressure.
- Repeatable assembly.
- Access for disassembly.

### Pressure generated during filling

Even manual syringe filling generates pressure inside the mold.

The force acting on the mold enclosure can be approximated by:

\[
F=P A
\]

Where:

- \(F\) = force acting on the enclosure.
- \(P\) = internal pressure.
- \(A\) = effective projected area.

This means that even a relatively small internal pressure can generate a significant separating force when acting over a large area.

The clamping system must therefore be evaluated according to the actual filling pressure, not simply the weight of the silicone.

The mold should be tested for leakage and deformation before the first complete casting operation.

---

# 03. SYRINGE-BASED SILICONE FILLING

## 3.1 Why use a syringe?

A syringe provides a controlled method of introducing uncured silicone into the mold.

Compared with gravity pouring, syringe filling allows the operator to control the material delivery rate and direct the silicone toward specific regions of the cavity.

This is particularly useful when the mold has restricted openings or complex internal geometry.

The syringe system must be compatible with the silicone viscosity and pot life.

A large-bore syringe or dispensing barrel is preferable to a narrow needle for viscous silicone.

A narrow nozzle can significantly increase flow resistance and the required injection force.

## 3.2 Syringe and nozzle selection

The syringe must provide sufficient capacity and allow controlled material delivery.

Relevant considerations include:

- Internal barrel diameter.
- Barrel capacity.
- Nozzle diameter.
- Nozzle length.
- Connection compatibility.
- Plunger force.
- Silicone viscosity.

A large-bore dispensing nozzle is preferable to a conventional hypodermic needle.

The objective is to minimize unnecessary restrictions between the syringe and mold cavity.

The nozzle should also connect securely to the mold inlet to prevent leakage.

## 3.3 Flow resistance

When viscous silicone passes through a restricted channel, it experiences resistance to flow.

For a simplified Newtonian fluid flowing through a cylindrical tube under laminar conditions, the Hagen–Poiseuille relationship is:

\[
Q=\frac{\pi r^4\Delta P}{8\mu L}
\]

Where:

- \(Q\) = volumetric flow rate.
- \(r\) = internal channel radius.
- \(\Delta P\) = pressure difference.
- \(\mu\) = dynamic viscosity.
- \(L\) = channel length.

This equation demonstrates an important relationship:

**Small changes in channel diameter can produce large changes in flow resistance.**

For example, reducing the channel radius increases resistance substantially.

The equation is an idealized model. Real silicone formulations may be non-Newtonian, and actual filling behavior depends on the material formulation, temperature and geometry.

Nevertheless, it illustrates why the inlet should avoid unnecessary restrictions.

## 3.4 Injection channel design

The injection channel must allow silicone to enter the mold without excessive pressure.

The design should prioritize:

- Short flow paths.
- Smooth internal transitions.
- Adequate cross-sectional area.
- Minimal sharp restrictions.
- Secure syringe connection.
- Easy cleaning or removal of cured material.

For the first prototype, the inlet diameter should be selected after checking the actual dispensing nozzle and silicone viscosity.

The previously considered Ø8 mm inlet is only a preliminary CAD reference, not a validated requirement.

A larger inlet may be appropriate depending on the dispensing equipment.

## 3.5 Injection funnel or connection port

Because the system uses a syringe, the original gravity-pouring funnel is no longer essential.

Instead, the mold should incorporate a suitable syringe connection.

Possible configurations:

- Straight cylindrical inlet.
- Tapered syringe adapter.
- Threaded connection.
- Replaceable dispensing nozzle.
- Short enlarged entry chamber.

A tapered connection may improve alignment between the syringe and the mold.

The connection must be sufficiently secure to prevent silicone escaping around the nozzle.

The injection port should also be positioned where the operator can access it without interfering with the clamping mechanism.

---

# 04. INJECTION PORT POSITIONING

## 4.1 Top, side or bottom inlet?

The injection port does not necessarily need to be positioned at the top.

Its position should be determined by the geometry of the cavity and the location of potential air traps.

For a syringe-fed system, a side or lower inlet can be useful when it allows silicone to advance through the cavity while displacing air toward upper vents.

### Bottom or lower-side injection

Potential advantages:

- Allows a rising filling front.
- Can direct air toward upper vent locations.
- May be suitable for cavities with a clear upward filling path.

Potential limitations:

- Requires suitable positioning and support.
- Can create long flow paths.
- May require additional vents.

### Top injection

Potential advantages:

- Easy syringe access in some configurations.
- Simple integration into the current CAD model.
- Suitable when the internal geometry supports progressive filling.

Potential limitations:

- Silicone can pass over recessed regions.
- Air may become trapped below overhanging geometry.
- Filling behavior may be less predictable in certain orientations.

### Current design direction

The existing top inlet can be retained for the first prototype if the cavity geometry and vent positions allow effective air evacuation.

However, the preferred arrangement should be evaluated using the actual master geometry.

The ideal configuration is one where the filling front moves progressively through the cavity and pushes air toward dedicated vent outlets.

---

# 05. AIR VENTING SYSTEM

## 5.1 Purpose of air vents

Air vents are essential because the silicone entering the mold must displace the air already occupying the cavity.

Without adequate venting, air can become trapped.

These trapped regions may produce:

- Internal voids.
- Missing surface details.
- Incomplete filling.
- Localized defects.
- Reduced dimensional accuracy.

The vent system must provide a path for air to escape throughout the filling operation.

## 5.2 Vent positioning

Vent positions should be selected according to the actual filling direction.

The main vent should generally connect to the region expected to fill last.

Additional vents may be necessary around:

- Deep recesses.
- Narrow channels.
- Upper corners.
- Localized pockets.
- Regions behind complex geometry.

A vent located in the wrong position may not effectively evacuate trapped air.

The CAD model should therefore be inspected in its intended filling orientation.

## 5.3 Vent dimensions

For the initial prototype, the following dimensions can be investigated:

| Feature | Preliminary dimension |
|---|---:|
| Primary vent channel | Ø1–1.5 mm |
| Larger vent option | Ø2 mm |
| External vent outlet | Approximately Ø2 mm |

These are experimental starting dimensions rather than fixed specifications.

The required vent diameter depends on:

- Silicone viscosity.
- Injection speed.
- Vent length.
- Cavity geometry.
- Filling pressure.

The objective is to allow air to escape without creating unnecessarily large silicone leakage paths.

## 5.4 Vent channels

A vent can be designed as a small passage connecting the cavity to the outside.

Possible geometries include:

- Cylindrical holes.
- Shallow grooves.
- Rectangular microchannels.
- Channels following the parting surface.

The channels should remain open during filling.

If a vent is too restrictive, air may remain trapped even when the mold has an external opening.

## 5.5 Injection and vent relationship

The injection and vent systems must work together.

The injection port introduces silicone.

The vents release displaced air.

The filling front should move toward the vent locations rather than surrounding isolated air pockets.

The following simplified arrangement illustrates the intended principle:

```text
       AIR VENT
          |
          v
   +----------------+
   |                |
   |   CAVITY       |
   |                |
   |                |
   +--------+-------+
            ^
            |
       SYRINGE INLET
```

This is a conceptual representation only. The actual vent arrangement must follow the master geometry.

---

# 06. MATERIAL PREPARATION AND MIXING

## 6.1 Two-component silicone

Many mold-making silicones consist of two components that must be mixed before use.

The manufacturer's specified mixing ratio must be followed accurately.

For a general two-component system:

\[
m_A : m_B = \text{Specified ratio}
\]

The ratio may be defined by mass or volume.

It must never be assumed.

Incorrect mixing can cause incomplete curing and inconsistent mechanical properties.

## 6.2 Mixing technique

The objective is to obtain a homogeneous mixture while minimizing the amount of air introduced.

Recommended procedure:

1. Measure the components accurately.
2. Combine them in a suitable container.
3. Mix thoroughly.
4. Scrape the container walls and bottom.
5. Avoid unnecessarily aggressive mixing.
6. Transfer the material into the syringe or dispensing barrel.

The transfer operation should also minimize air introduction.

## 6.3 Pot life

Pot life is the available working time before the silicone becomes too viscous for the intended process.

This parameter is especially important for syringe filling.

The complete operation, including mixing, transfer and injection, must be performed within the manufacturer's specified working time.

The syringe and nozzle should not be allowed to remain filled with curing silicone longer than necessary.

---

# 07. VACUUM DEGASSING

## 7.1 What is degassing?

Vacuum degassing removes air incorporated into the silicone during mixing.

When the pressure surrounding the silicone is reduced, trapped bubbles expand and can escape from the liquid.

This helps reduce internal voids in the cured material.

## 7.2 Degassing versus mold venting

These processes have different functions.

| Process | Purpose |
|---|---|
| Vacuum degassing | Removes air from the mixed silicone |
| Mold venting | Releases air from the mold cavity during filling |

Vacuum degassing does not replace mold venting.

Similarly, a well-vented mold does not eliminate bubbles introduced during mixing.

Both systems can contribute to better results.

## 7.3 Process considerations

Vacuum degassing should follow the silicone manufacturer's recommendations.

The mixing container must have sufficient free volume because silicone can expand significantly under vacuum.

The material should be degassed before transfer into the syringe when the processing instructions permit it.

If no vacuum equipment is available, controlled mixing and transfer become especially important.

---

# 08. CURING PROCESS

## 8.1 Chemical curing

Silicone curing involves the formation of a crosslinked polymer network.

During this process, the liquid material transforms into an elastomer.

The exact chemical mechanism depends on the silicone formulation.

Common systems include:

- Condensation-cure silicone.
- Addition-cure silicone.

These formulations have different chemical characteristics and compatibility requirements.

## 8.2 Important curing parameters

The following information must be obtained from the selected silicone datasheet:

- Mixing ratio.
- Working time.
- Recommended curing temperature.
- Demolding time.
- Full curing time.
- Hardness after cure.
- Compatibility restrictions.

The mold must remain stationary during curing.

Opening the mold before the silicone has developed sufficient mechanical strength can cause deformation or tearing.

---

# 09. DEMOLDING AND EXTRACTION MECHANICS

## 9.1 Extraction architecture

The mold is designed so that the two outer halves open before the central insert is removed.

This provides access to the master carrier and reduces the possibility of interference.

The intended sequence is:

1. Allow the silicone to cure.
2. Release the custom clamping mechanism.
3. Open the left and right outer halves.
4. Remove the central insert with the master.
5. Separate the master from the silicone negative.

## 9.2 Undercuts

Undercuts are features that prevent straight-line extraction.

They are particularly important because the selected Shore A 55 silicone is relatively firm compared with softer mold-making formulations.

The silicone must deform sufficiently to release the master without tearing.

The geometry must therefore be evaluated for:

- Reverse-facing surfaces.
- Recessed features.
- Sharp internal corners.
- Narrow passages.
- Mechanical interference.

The actual tear strength and elongation of the selected silicone are more useful than hardness alone when evaluating difficult demolding conditions.

## 9.3 Mechanical extraction assistance

The current design includes the possibility of using two extraction points.

The purpose is to distribute the force applied to the central insert.

Two symmetrical extraction points can help reduce tilting when both are operated evenly.

A possible arrangement uses threaded M5 interfaces with jack screws.

The screws must push against reinforced areas of the carrier.

They must not apply force directly to the master or thin printed walls.

The extraction system must be tested before the silicone casting operation.

---

# 10. 3D PRINTED MOLD QUALITY

## 10.1 Surface integrity

FDM-printed parts contain layer interfaces and may contain microscopic gaps.

These gaps can allow liquid silicone to escape.

The printed mold should be inspected for:

- Layer separation.
- Surface defects.
- Gaps around interfaces.
- Poor dimensional accuracy.
- Incomplete sealing surfaces.

## 10.2 Wall thickness and rigidity

The mold enclosure must resist the loads generated during assembly and syringe filling.

Particular attention should be given to:

- Thin enclosure walls.
- Injection port surroundings.
- Vent passages.
- Clamping interfaces.
- Extraction holes.
- Alignment features.

The actual wall thickness should be selected according to the printed material, printing orientation and expected pressure.

## 10.3 Sealing

Sealing is especially important in a syringe-fed system.

The silicone must not leak through:

- The outer parting line.
- The central insert interface.
- The syringe connection.
- Unsealed printed surfaces.

The assembled mold should be inspected and tested before introducing the silicone.

---

# 11. PRELIMINARY DESIGN PARAMETERS

The following values summarize the current design considerations.

They are preliminary experimental references, not validated manufacturing specifications.

| Parameter | Current design direction |
|---|---|
| Cured silicone hardness | Shore A 55 |
| Filling method | Manual syringe |
| Mold architecture | Three-piece assembly |
| Outer structure | 3D printed |
| Master support | Removable central insert |
| Injection port | Short, unrestricted connection |
| Syringe nozzle | Large-bore dispensing tip |
| Primary vent | Ø1–1.5 mm starting range |
| Larger vent option | Ø2 mm |
| Extraction points | Two symmetrical points |
| Extraction interface | M5 under evaluation |
| Filling orientation | To be validated |
| Vacuum degassing | Optional process improvement |

**Important:** The final inlet diameter must be selected based on the syringe connection and uncured silicone viscosity. The vent dimensions must be validated through actual filling tests.

---

# 12. FIRST PROTOTYPE — MANUFACTURING PROCEDURE

## Phase 01 — CAD validation

- [ ] Verify the mold enclosure.
- [ ] Verify the central insert geometry.
- [ ] Check the master mounting interface.
- [ ] Verify the extraction direction.
- [ ] Check potential undercuts.
- [ ] Inspect injection channel geometry.
- [ ] Inspect vent locations.
- [ ] Check all sealing interfaces.
- [ ] Verify the custom clamping system.
- [ ] Check structural wall thickness.

## Phase 02 — 3D printing

- [ ] Manufacture all mold components.
- [ ] Inspect dimensional accuracy.
- [ ] Remove printing defects.
- [ ] Verify alignment.
- [ ] Test the clamping mechanism.
- [ ] Test opening and extraction without silicone.
- [ ] Inspect the syringe connection.
- [ ] Verify that the vents are unobstructed.

## Phase 03 — Silicone preparation

- [ ] Select the Shore A 55 formulation.
- [ ] Obtain the technical datasheet.
- [ ] Verify uncured viscosity.
- [ ] Confirm mixing ratio.
- [ ] Calculate material quantity.
- [ ] Verify pot life.
- [ ] Verify curing time.
- [ ] Check material compatibility.
- [ ] Prepare syringe and dispensing nozzle.
- [ ] Prepare vacuum equipment if available.

## Phase 04 — Syringe filling

- [ ] Assemble the mold.
- [ ] Verify the clamping system.
- [ ] Confirm that the injection port is sealed.
- [ ] Confirm that vents are open.
- [ ] Mix the silicone.
- [ ] Degas if applicable.
- [ ] Transfer silicone into the syringe.
- [ ] Connect the syringe to the inlet.
- [ ] Introduce silicone gradually.
- [ ] Monitor vent outlets.
- [ ] Confirm complete filling.
- [ ] Stop if abnormal pressure or leakage occurs.

## Phase 05 — Curing and extraction

- [ ] Keep the mold stationary.
- [ ] Follow the manufacturer's curing conditions.
- [ ] Allow sufficient curing time.
- [ ] Open the outer halves.
- [ ] Remove the central insert.
- [ ] Extract the master carefully.
- [ ] Inspect the silicone negative.
- [ ] Document defects.

---

# 13. FAILURE ANALYSIS

| Problem | Possible cause | Engineering response |
|---|---|---|
| High syringe resistance | Narrow inlet or high viscosity | Increase flow area or shorten the inlet |
| Silicone leaking | Poor sealing or excessive pressure | Improve interfaces and filling control |
| Trapped air | Incorrect vent positioning | Relocate or add vents |
| Incomplete filling | Excessive flow resistance | Review channel geometry |
| Surface bubbles | Air introduced during mixing | Improve mixing or degas |
| Incomplete curing | Incorrect mixing or chemical inhibition | Check datasheet and compatibility |
| Master difficult to remove | Undercuts or insufficient flexibility | Review geometry and material properties |
| Silicone tearing | Excessive extraction stress | Improve extraction strategy |
| Mold deformation | Insufficient structural rigidity | Reinforce printed components |
| Excessive flash | Gaps between mold components | Improve sealing and alignment |

---

# 14. EXPERIMENTAL VALIDATION

The first prototype will be used to validate the mechanical assembly and syringe-filling system.

The following information should be recorded during testing.

| Variable | Measurement |
|---|---|
| Silicone manufacturer | Product identification |
| Shore hardness | Shore A 55 target |
| Uncured viscosity | Datasheet value |
| Mixing ratio | Manufacturer specification |
| Material quantity | Grams |
| Pot life | Minutes |
| Curing time | Hours |
| Syringe capacity | mL |
| Syringe nozzle diameter | mm |
| Injection channel diameter | mm |
| Vent diameter | mm |
| Filling orientation | Description |
| Filling behavior | Observations |
| Leakage | Yes / No |
| Air pockets | Yes / No |
| Extraction difficulty | Observations |
| Final mold quality | Pass / Fail |

The first test should focus on obtaining a complete, defect-free silicone negative rather than optimizing production speed.

After the initial results, inlet geometry, vent positioning and mechanical design can be adjusted independently.

---

# 15. ENGINEERING KNOWLEDGE REQUIRED

Before manufacturing the first prototype, I need to understand the following principles.

### Fluid mechanics

- Viscosity.
- Pressure and flow rate.
- Hagen–Poiseuille relationship.
- Laminar flow.
- Flow restrictions.
- Hydrostatic pressure.
- Air displacement.

### Polymer science

- Silicone chemistry.
- Crosslinking.
- Addition and condensation curing.
- Elastomer behavior.
- Shore hardness.
- Tear strength.
- Elongation at break.
- Material compatibility.

### Mechanical engineering

- Draft angles.
- Undercuts.
- Parting lines.
- Mechanical tolerances.
- Alignment systems.
- Clamping forces.
- Extraction forces.
- Structural rigidity.

### Manufacturing engineering

- FDM printing.
- Surface finishing.
- Sealing techniques.
- Dimensional inspection.
- Process repeatability.
- Design for Manufacturing.

---

# 16. FUTURE DEVELOPMENT

Once the first prototype has been validated, the following improvements can be investigated:

- Optimization of syringe connections.
- Alternative injection channel geometries.
- Improved vent distribution.
- Reduced silicone consumption.
- Better master positioning.
- Improved central insert extraction.
- Alternative Shore hardness formulations.
- Vacuum degassing integration.
- Improved sealing methods.
- Repeatability testing.

The long-term objective is to establish a controlled and repeatable silicone mold manufacturing process for custom Tuka Customs components.

---

# 17. REFERENCES AND TECHNICAL DOCUMENTATION

The following references will support the theoretical development of this project.

1. **Silicone manufacturer technical datasheets** — Viscosity, mixing ratio, pot life, curing time, hardness and mechanical properties.
2. **Silicone processing guides** — Mixing, degassing, dispensing and demolding.
3. **ASTM D2240** — Standard Test Method for Rubber Property: Durometer Hardness.
4. **ASTM D624** — Standard Test Method for Tear Strength of Conventional Vulcanized Rubber and Thermoplastic Elastomers.
5. **Fluid Mechanics textbooks** — Pressure, viscosity, flow resistance and fluid transport.
6. **Polymer Science references** — Elastomer chemistry and crosslinking.
7. **Additive Manufacturing references** — FDM printing, dimensional accuracy and structural properties.

Specific material datasheets must be added once the selected silicone formulation is confirmed.

---

# 18. DEVELOPMENT LOG

| Revision | Description | Status |
|---|---|---|
| 01 | Initial mold architecture and gravity-pouring study | Superseded |
| 02 | Syringe-based filling and Shore A 55 study | Current |
| 03 | CAD design validation | Pending |
| 04 | First printed prototype | Pending |
| 05 | First syringe-filling experiment | Pending |
| 06 | Inspection and design optimization | Pending |
| 07 | Validated manufacturing procedure | Pending |

---

<p align="center">

**TUKA CUSTOMS™**

*Engineering through experimentation.*

`RESEARCH` · `DESIGN` · `MANUFACTURE` · `VALIDATE`

**END OF DOCUMENT // REV. 02**

</p>
