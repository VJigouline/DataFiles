# Robot and CNC Model References (STEP)

Sources of free STEP files for industrial robots and CNC machines, collected for testing
model import, robot simulation and machine programming.

Links checked on 2026-11-09. The models are **not** part of this repository and are **not**
covered by its MIT License: each one has its own license or terms of use, which must be
checked before use or redistribution.

## Official manufacturer models

Accurate geometry, usually free after registration.

| Manufacturer | Models | Source | Notes |
|---|---|---|---|
| Universal Robots | UR3e, UR5e, UR10e, UR20 and others | [universal-robots.com/download](https://www.universal-robots.com/download/) | Free STEP files for every model. Each axis is a separate solid, which makes the joints easy to rig. |
| ABB | IRB 1200, IRB 4600, IRB 6700 and others | ABB Robotics product pages | CAD download (STEP) on each robot's product page. |
| KUKA | KR series | [KUKA downloads](https://www.kuka.com/en-de/services/downloads) | Free registration (my.kuka.com). |
| FANUC | All arms | FANUC CAD portal / ROBOGUIDE | Account required. |
| Yaskawa Motoman | All arms | motoman.com (search "CAD models") | Free, request form. |
| DENSO | All arms | [DENSO CAD download guide](https://support.densorobotics.com/en/support/solutions/articles/60000697367-where-can-i-download-cad-files-for-robot-) | Explains where to download the CAD files. |

## Community libraries

Third-party uploads: check accuracy, completeness and license for each model.

| Robot | Format | Source |
|---|---|---|
| ABB IRB 6700 | STEP AP203, ~7 MB, free | [CGTrader](https://www.cgtrader.com/free-3d-models/industrial/industrial-machine/abb-articulated-robot-irb-6700) |
| ABB IRB 4600 | STEP, ~6.7 MB, free | [CGTrader](https://www.cgtrader.com/free-3d-models/industrial/industrial-machine/abb-articulated-robot-irb-4600) |
| ABB IRB 1600ID | STEP, IGES | [3DCadBrowser](https://www.3dcadbrowser.com/3d-model/abb-irb-1600id-6-axis-robot) |
| KUKA KR 1000 Titan | STEP, free | [CGTrader](https://www.cgtrader.com/free-3d-models/industrial/industrial-machine/kr-1000-titan) |
| KUKA KR 600 Fortec | Free, formats not listed | [CGTrader](https://www.cgtrader.com/free-3d-models/industrial/industrial-machine/kr-600-fortec) |
| KUKA KR 3 | Free, formats not listed | [CGTrader](https://www.cgtrader.com/free-3d-models/industrial/industrial-machine/kr-3-robot) |
| KUKA KR210 | Free account | [3DCadBrowser](https://www.3dcadbrowser.com/3d-model/kuka-robot-kr210) |
| FANUC R-2000iB/125L | STEP, free account | [3DCadBrowser](https://3dcadbrowser.com/3d-model/fanuc-r-2000ib125l-robot-arm) |
| FANUC M-10iA | Free account | [3DCadBrowser](https://3dcadbrowser.com/3d-model/fanuc-m10ia-robot-arm-6-axis) |
| Tormach robot | Zipped STEP (full arm) + tool flange | [Tormach wiki](https://tormach.atlassian.net/wiki/spaces/ROBO/pages/2112094580/3D+Models) |

## Open-source robot arms

| Robot | Source | Notes |
|---|---|---|
| Thor (6-axis, 3D-printable) | [github.com/AngelLM/Thor](https://github.com/AngelLM/Thor) | 72 STEP files in the repo, plus FreeCAD sources (`freecad-src/*.fcstd`) for every part. |
| BCN3D Moveo (5-axis) | [github.com/BCN3D/BCN3D-Moveo](https://github.com/BCN3D/BCN3D-Moveo) | `CAD files` folder; no `.step` files found, so it may be in another CAD format. |

## Open-source CNC machines

| Machine | Source | Notes |
|---|---|---|
| Sienci LongMill / AltMill | [resources.sienci.com](https://resources.sienci.com/view/lm-advanced/) | GPLv3. Designs on Onshape, exportable as STEP, IGES or STL. |
| Open Source Desktop CNC Router | [MakerWorld](https://makerworld.com/en/models/3130212-open-source-desktop-cnc-router-final-version) | Free CAD files. No `.step` files found in its GitHub repo. |

## Recommendation

- **Robot simulation:** Universal Robots STEP files (official, free, one solid per axis).
- **No license restrictions:** Thor (open source, STEP and FreeCAD sources).
- **Loading STEP in the browser:** [occt-import-js](https://github.com/kovacsv/occt-import-js) (OpenCascade compiled to WebAssembly) converts STEP and IGES to meshes for three.js.
