# DoomCube-2

A Voron 2.4 rebuilt as a [DoomCube-2](https://github.com/FrankenVoron/DoomCube-2).

**Recorded print time:** 3,746 hours on the mechanical hour counter. This is a recorded reading, not a live total.

## Build and modifications

| Component | Installed hardware / notes | Reference |
| --- | --- | --- |
| Base printer | Voron 2.4 | [Voron 2.4](https://github.com/VoronDesign/Voron-2) |
| Rebuild | DoomCube-2 | [DoomCube-2 project](https://github.com/FrankenVoron/DoomCube-2) |
| Main controller | FYSETC Spider v2 PCB | [FYSETC Spider project](https://github.com/FYSETC/FYSETC-SPIDER) |
| Toolhead board | Voron Afterburner Toolhead PCB — Complete — V3.rabbit — ERCF | [Board listing](https://kb-3d.com/store/electronics/357-voron-afterburner-toolhead-pcb-complete-v3rabbit-ercf-1634426646789.html) · [Afterburner PCB project](https://github.com/VoronDesign/Voron-Hardware/tree/master/Afterburner_Toolhead_PCB) |
| Magnetic Z probe | Annex Engineering magnetic probe; likely Quickdraw, exact identity to confirm | [Quickdraw probe](https://github.com/Annex-Engineering/Quickdraw_Probe) |
| Z endstop | Sexbolt Z endstop | Exact design/revision link to add |
| Automatic Z calibration | Klipper-based automatic Z calibration; installed firmware and module to confirm | [Automatic Z-calibration plugin for Klipper](https://github.com/protoloft/klipper_z_calibration) |
| Hour counter | Mechanical counter; recorded reading of 3,746 print hours | Model and wiring to add |
| Expansion PCB | Voron expansion PCB; exact board/revision to confirm | [Klipper Expander reference](https://github.com/VoronDesign/Voron-Hardware/tree/master/Klipper_Expander) |
| Enclosure lighting | LED lights | Model and wiring to add |
| Enclosure camera | Camera inside the enclosure | Model and mounting details to add |
| Nozzle cleaning | Toolhead brush | Design and cleaning macro to add |
| Bed fans | Installed | Fan layout and control configuration to add |
| Air filter | Nevermore carbon air filter; model/revision to confirm | [Nevermore Micro project](https://github.com/nevermore3d/Nevermore_Micro) |

The ERCF designation identifies the toolhead board variant; an ERCF feeder has not been recorded as part of this build. Links for components with an unconfirmed model are references, pending identification of the installed hardware.

## Photos

[Photo directory](photos/README.md) — photos have not been added yet. Add original photos here and embed them in this index with relative paths.

## Configuration

[Configuration backup](config/config.tgz) — supplied printer configuration, with two Home Assistant token values redacted. See the [configuration notes](config/README.md) for archive contents and restoration details. The backup contains `quickdraw_probe.cfg` and a `[z_calibration]` section; the firmware fork and version remain unconfirmed.

Automatic Z calibration is available as a Klipper plugin, so the feature is not exclusive to Danger Klipper. The firmware fork, version, and calibration implementation actually running on this printer still need to be recorded.

## Details to capture

- Firmware version/commit and installed extensions.
- Full-printer, toolhead, probe/endstop, electronics, and enclosure photos.
- Confirmation of the Annex probe and expansion PCB models.
- Build volume, hotend, extruder, and rebuild date.
- Exact designs or part references for the remaining modifications.
