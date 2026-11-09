# CNC Machine Tool Model References (STEP)

Sources of free STEP files for CNC milling machines, collected for testing model import,
machine simulation and CNC programming.

Links and files checked on 2026-11-09. The models are **not** part of this repository and are
**not** covered by its MIT License: each one has its own license or terms of use, which must be
checked before use or redistribution.

See also [Robots](../Robots/README.md) for industrial robot models.

## Complete machine models (open source)

[Mekanika EVO](https://github.com/mekanika-dev/evo): open-source gantry-type 3-axis CNC milling
machine. Each file is a full machine assembly (frame, axes, spindle mount, hardware). The repo
also contains the bill of materials (`bom/`) and assembly docs (`docs/`).

| Model | File | Size | License |
|---|---|---|---|
| EVO-S (small) | [EVO-S V1.0.stp](https://github.com/mekanika-dev/evo/blob/main/cad/EVO-S%20V1.0.stp) | 93 MB | CERN-OHL-S-2.0 |
| EVO-M (medium) | [EVO-M V1.0.stp](https://github.com/mekanika-dev/evo/blob/main/cad/EVO-M%20V1.0.stp) | 93 MB | CERN-OHL-S-2.0 |
| EVO-L (large) | [EVO-L V1.0.stp](https://github.com/mekanika-dev/evo/blob/main/cad/EVO-L%20V1.0.stp) | 93 MB | CERN-OHL-S-2.0 |
| EVO-CU | [EVO-CU V1.0.step](https://github.com/mekanika-dev/evo/blob/main/cad/EVO-CU%20V1.0.step) | 76 MB (Git LFS) | CERN-OHL-S-2.0 |

CERN-OHL-S-2.0 allows any use, but modified versions of the design must be shared under the
same license. Copyright © 2025 Mekanika SRL.

## Other open-source mills

Individual parts only, or other CAD formats.

| Machine | Source | License | Notes |
|---|---|---|---|
| CARVER X5 (5-axis) | [github.com/MakerLabTunisia/CARVER_X5](https://github.com/MakerLabTunisia/CARVER_X5) | CC-BY-SA-4.0 | Design in SolidWorks (`.SLDPRT` / `.SLDASM`); only one STEP part. Needs SolidWorks or a converter to export STEP. |
| Milo v1.5 (desktop mill) | [github.com/bazil14/Milo-v1.5](https://github.com/bazil14/Milo-v1.5) | See repo | Only 2 STEP plates; the rest is STL. |
| X-Carve-based mill | [github.com/jduanen/X-Carve](https://github.com/jduanen/X-Carve) | See repo | 7 STEP accessories (dust shoe, rings), not the full machine. |
| Sienci LongMill / AltMill | [resources.sienci.com](https://resources.sienci.com/view/lm-advanced/) | GPLv3 | Design on Onshape, exportable as STEP, IGES or STL. |

Background: [Comparison of Open-Source Desktop CNC Mill Designs](https://fab.cba.mit.edu/classes/863.23/EECS/people/Ahmad/CNC-Mill/Comparison%20of%20Open-Source%20Desktop%20CNC%20Mill%20Designs.pdf) (MIT Fab Lab).

## Industrial machines

| Machine | Source | Notes |
|---|---|---|
| iSEL CNC milling machines | [iSEL CAD downloads](https://www.isel.com/en/support-downloads/cad-downloads-step-and-dfx-data/3d-data-systems.html) | Official manufacturer models, free. STEP files under each machine's **Downloads** tab. |
| VMC BT40 vertical machining center | [stlfinder (GrabCAD mirror)](https://stlfinder.com/model/vmc-vertical-milling-center-bt40-wnZmvVI2/402442) | Full assembly as STEP. Check the license on the original GrabCAD page. |
| Milling machine | [3DCadBrowser](https://www.3dcadbrowser.com/3d-model/milling-machine-72031) | STEP and IGES. Check whether it is free. |

## Paid models

| Machine | Source |
|---|---|
| CNC vertical machining center | [CGTrader](https://www.cgtrader.com/3d-models/industrial/industrial-machine/cnc-vertical-machining-center-3d-model-industrial-mill) |
| 5-axis CNC machine | [CGTrader](https://www.cgtrader.com/3d-models/industrial/industrial-machine/5-axis-cnc-machine) |
| 6-axis CNC milling machine | [CGTrader](https://cgtrader.com/3d-models/industrial/machine/six-axis-cnc-milling-machine) |

Prices range from about $10 to $76.

## Recommendation

- **Testing:** Mekanika EVO-S, a complete open-source machine assembly.
- **Real commercial machine geometry:** iSEL.
- **Large-file stress test:** the 93 MB EVO files. In the browser, run
  [occt-import-js](https://github.com/kovacsv/occt-import-js) in a Web Worker so the page does
  not freeze during conversion.
