# Layout optimisation

One plate evaporator remains. The condenser is direct air cooled with no condenser coolant loop. Only the fan/condenser enclosure wall is present.

| Measured CAD quantity | Before | Revised |
|---|---:|---:|
| Width × height × depth, mm | 572 × 500 × 687 | 490 × 500 × 672 |
| Total tube centreline length, mm | 3071.8 | 2926.4 |
| Modelled bends | 22 | 20 |

The model bounding footprint is 16.2% smaller. Tube length is 4.7% lower. These figures exclude installation access, external heat-source equipment and unmodelled services.

Changes: hot-water pump moved onto the right side of the equipment baseplate at X152/Y26/Z25 mm; fan/condenser group moved 15 mm forward; R1 overhead routing lowered and resequenced; R2 removes one offset bend; W1 uses a single bend aligned to its evaporator port; W2 moved closer to the evaporator to clear the hot-water pump; R4/R5 shortened to the new condenser position. Evaporator and drivetrain placements stay fixed to retain their current interfaces. The baseplate now supports the hot-water pump envelope, but its mounting holes/fasteners remain to be designed.

Verification: see Native_QA.txt and Pipe_Clearance_Screen.json. Tube centreline lengths are layout lengths, not fabrication cut lengths. This is a geometric packing improvement, not a proof of a global optimum, pressure-drop improvement or thermal performance. Space for actual fittings, insulation, tools and component removal must be checked against selected supplier parts. Tight inherited bends and unvalidated tube dimensions remain draft. The inherited shaft overlap and support/coupling details remain unresolved. Fan/condenser sizing, refrigerant rating and the ₹15,000 budget are still unverified.
