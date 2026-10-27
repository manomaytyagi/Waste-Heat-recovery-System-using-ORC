# CAD Final — optimised direct air-cooled ORC layout

**One plate heat exchanger remains: the evaporator. There is no plate condenser and no condenser cooling-water loop.**

Open **ORC_Optimised_Single_Wall.SLDASM** in SolidWorks 2026. Keep all subfolders together. The matching **STEP** is the neutral assembly export, and **ORC_Air_Cooled_Isometric.png** is the single isometric image.

## Corrected circuit

Receiver → refrigerant feed pump → **plate evaporator** → expander → **air-cooled refrigerant condenser + fan** → receiver.

The plate evaporator's hot-water heat-input circuit and its baseplate-mounted pump remain. These are not condenser-cooling components.

The enclosure has only the condenser/fan wall. The equipment baseplate remains; the other walls and enclosure floor are absent.

## Organized files

| Folder | Contents |
|---|---|
| Assembly Parts | Single wall, baseplate, supports, seats, risers, shroud, mounts and guard |
| Pipe Parts | Five refrigerant runs, two evaporator hot-water runs, and evaporator adapters |
| Components | One plate evaporator, air-cooled refrigerant condenser, fan, expander, generator, receiver and retained pumps/motor |
| Documentation | Parts list, quantities, placements, pipe schedule, build notes and verification |

There are **31 assembly instances and 29 unique parts**. Each unique part has a native **SLDPRT** and a matching **STEP**. The assembly uses fixed layout placements, not production mates. Individual part exports use local coordinates; the placement schedule provides translations in millimetres.

## Release status

This corrects the cooling architecture and supersedes the previous coolant-loop package. The old automotive coolant-radiator recommendation is withdrawn for this design. A **refrigerant-rated air-cooled condenser**, suitable for the actual ORC fluid, pressure, temperature and heat duty, must be selected.

The new condenser and fan are provisional envelopes, not approved purchased equipment. The previous ₹15,000 condenser/fan budget remains a target; no verified replacement condenser/fan quotation is included. Do not use the earlier ₹5,810 car-radiator/fan subtotal for this design.

“CAD Final” is the handoff-folder name, not a manufacturing release. Read **Documentation/Build_Notes.md** for the remaining fabrication and engineering items, including the inherited expander/generator shaft overlap.


## Layout revision

See [Optimisation_Report.md](Documentation/Optimisation_Report.md) for measured before/after dimensions and piping changes. The hot-water pump now sits on the baseplate. This package is a separate revision; the previous CAD has been retained.
