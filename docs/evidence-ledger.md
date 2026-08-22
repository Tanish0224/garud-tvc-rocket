# GARUD Project Evidence Ledger

This ledger tracks the provenance and verification status of all claims in the GARUD project case study.

## Classification Key
- **A. DIRECTLY VERIFIED**: Supported by inspecting local engineering files (CAD, simulations, datasets, images).
- **B. VERIFIED FROM USER-SUPPLIED CONTEXT**: Explicitly provided and verified by the user's project summary.
- **C. SUPPORTED BUT NEEDS REVIEW**: Evidenced in source files but requires human confirmation before publication.
- **D. UNCERTAIN / DO NOT PUBLISH YET**: Mentioned or implied but lacks explicit verification.

## Fact Ledger

| Claim | Verification Status | Source / Provenance |
|-------|---------------------|---------------------|
| **Project objective**: Develop a thrust-vector-controlled model rocket for controlled ascent and retro-thrust-assisted landing. | B. VERIFIED FROM USER-SUPPLIED CONTEXT | User-supplied context |
| **Team Leadership**: Led a four-member team coordinating design, avionics, fabrication, and assembly. | B. VERIFIED FROM USER-SUPPLIED CONTEXT | User-supplied context |
| **Mechanical Design**: Primary ownership of TVC mechanism and landing-leg assembly design using Fusion 360 and SOLIDWORKS. | A. DIRECTLY VERIFIED | Local files: `TVC_Mount.f3z`, `Landing-Legs v10.f3d`, `R3 v3.step` |
| **TVC Mechanism**: Integrated dual-servo actuation for multi-axis thrust vectoring. | B. VERIFIED FROM USER-SUPPLIED CONTEXT | User-supplied context; CAD files indicate 2-axis gimbal mounts (`Inner Gimbal`, `Outer Gimbal`) |
| **Control Logic & Simulation**: The team simulated trajectory and developed PID-based thrust-vector control logic in MATLAB/Simulink and RockSim. | B. VERIFIED FROM USER-SUPPLIED CONTEXT | User-supplied context |
| **Fabrication (3D Printing)**: 3D-printed the TVC and landing assemblies with the team. | A. DIRECTLY VERIFIED | Local files: `.stl` export directories (`3D-Print/TVC-New/`), `Ultimaker1.png` |
| **Physical Integration**: Integrated the TVC and landing-leg systems into the rocket; system-level assembly performed with the team. | A. DIRECTLY VERIFIED | User-supplied context; Local files: `LG-1.jpg`, `LG-2.jpg` (hardware photos) |

## Claims Requiring Human Review (Status C/D)
- *Specific peak altitude, apogee, or max velocity numbers (no hard numbers provided in user context, defer to thesis or withhold).*
- *The exact PID tuning parameters and simulation outputs require validation against final test data if they are to be published.*

## Evidence Manifest
- `Rocket_Thesis_Final.pdf`: Final project report
- `Mass-Time_Rocket.xlsx`: Propulsion/mass modeling
- `TVC_Mount.f3z`, `Landing-Legs v10.f3d`: Core CAD
- `R5_Ascent.png`, `R6-Descent-2.png`: Visual evidence of trajectory/design phases
- `LG-1.jpg`, `LG-2.jpg`: Physical prototype evidence
