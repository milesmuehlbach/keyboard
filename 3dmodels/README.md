# Board 3D models

All PCB model paths use `${KIPRJMOD}/3dmodels`, so this directory travels with the project. The original model placements are preserved except for the replacement encoder and newly assigned spacebar stabilizer. `DAS 1.25u` was corrected to `DSA 1.25u`.

Sources and download checksums are recorded in [sources.json](sources.json). Included upstream licenses are in [licenses](licenses).

- DSA keycaps: https://github.com/anhthang/dsa-keycap (MIT).
- Cherry MX switch and 2u stabilizer: https://github.com/monotech/Osborne1-KeyboardReplacement (repository GPL-3.0; original CAD author/license is not separately identified).
- Diode and Pico variants: https://gitlab.com/kicad/libraries/kicad-packages3D (see bundled KiCad license).
- Encoder: https://gitea.mcflyer.ru/McFLY/kicad_libs/commit/01f41db82306013ce1139556f2b2bf83afdd0a1e. KiCad's referenced EC11E STEP file is absent upstream. This community switched EC11 model is positioned at the footprint shaft center and rotated to match the terminal layout. It is an approximate visual replacement: shaft height and detailed dimensions may differ from the selected Alps part. No separate model license was found in the source.
- `Stabilizer 6.25u.step` is derived from the downloaded stabilizer assembly: right housings translated and wire stretched along X to match the footprint's 100.0125 mm housing spacing. Treat it as a visualization model.

Disabled Pico variant models remain disabled. Logos and mounting holes need no component model.
