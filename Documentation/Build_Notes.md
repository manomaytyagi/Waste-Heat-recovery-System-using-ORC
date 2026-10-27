# Build notes — corrected direct air cooling

## Authoritative configuration

The plate **evaporator stays**. The plate **condenser is removed**. Expander exhaust now enters the air-cooled refrigerant condenser directly; condensed refrigerant returns to the liquid receiver. There is no secondary condenser coolant loop or coolant circulation pump.

Removed from this package: second plate exchanger, its seat, its four adapters, W3/W4/W5 coolant pipes, inline coolant pump and automotive water-radiator model. The evaporator, hot-water pump, W1/W2 hot-water lines and evaporator adapters remain.

R4 is expander → air-cooled condenser. R5 is air-cooled condenser → receiver. All seven routes are native hollow sweeps. R2 and W1 have fewer bends; R4 and R5 match the closer condenser wall.

## Condenser model and interfaces

**OF_Air_Cooled_Refrigerant_Condenser_UNSELECTED** is new generic layout geometry. It is not the selected Alto water radiator relabelled as suitable for refrigerant. Rectangular headers, tubes and fins are schematic external geometry; actual internal circuiting and pressure boundaries are not designed.

- Reserved overall header envelope: X = −225…225 mm, Y = 40…445 mm, Z = 270…320 mm.
- Proposed vapour connection tube end: X = −55, Y = 420, Z = 255 mm; provisional 18 mm OD / 16 mm ID route.
- Proposed liquid connection tube end: X = −30, Y = 64, Z = 255 mm; provisional 8 mm OD / 6 mm ID route.
- Port positions and header geometry are assumed, to be replaced with supplier CAD.
- The fan, shroud, mounts and guard remain provisional. Their continued geometric fit does not establish condenser thermal performance or fan suitability.

Select a refrigerant condenser for the actual working fluid (previous design basis: R245fa), design pressure/temperature, mass flow, heat rejection and ambient temperature. Verify refrigerant pressure drop, subcooling and fan power. The existing automotive coolant-radiator price shortlist is not applicable to this direct-refrigerant circuit. No purchase-ready condenser selection or verified ₹15,000 combination is claimed.

The liquid route rises from the assumed lower condenser outlet to the receiver's existing top inlet. Confirm the required pressure head, drainage and liquid seal behaviour; change the receiver connection/relative heights or condenser outlet arrangement if required by the selected system. This layout is not evidence that gravity drainage or stable condensation is assured.

## Single wall and structural work

The retained single wall is 490 × 500 × 2 mm with a 340 mm fan aperture, at Z = 363…365 mm. All these dimensions remain draft. A separate common frame or bench attachment is needed: removing the enclosure floor and other walls removes their possible support contribution. Condenser mounting feet lie behind the retained equipment baseplate and are not shown attached to a validated support frame.

Finalize materials, wall thickness, fasteners, isolators, mounting holes, shroud sealing and guarding after receiving verified equipment dimensions. Fan blades and guard geometry are illustrative, not certified protective designs.

## Other retained limitations

- Resolve the inherited expander/generator shaft overlap and select couplings before manufacture. The feed-pump motor coupling and support attachments also remain incomplete.
- Tube sizes, walls and bend radii remain provisional; tight bends may need fittings. Establish pressure ratings, materials/seal compatibility, pressure loss and workshop cut lengths after selecting connections.
- Confirm feed-pump and receiver suitability for the refrigerant and duty, plus the hot-water pump's continuous temperature rating.
- Heat source/reservoir, refrigerant relief/service provisions, instrumentation and electrical controls are not fully modelled.

## Handoff and verification

Use `Parts_List.csv` for quantities and paired native/STEP files. `Assembly_Placements.csv` gives local-origin translations into assembly coordinates; unchanged orientations are retained. `Tube_Centerlines.json` uses assembly millimetres, and `Tube_Schedule.csv` lists centreline lengths rather than shop cut lengths.

`Pipe_Clearance_Screen.json` is a sampled pipe-to-pipe check. `Native_QA.txt` records SolidWorks' assembly interference results, excluding coincident contact and interference between bodies inside the same part. Neither establishes pressure, thermal, structural or fabrication readiness.
