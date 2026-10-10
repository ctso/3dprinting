# DoomCube-2

My Voron 2.4, rebuilt as a [DoomCube-2](https://github.com/FrankenVoron/DoomCube-2).

<img src="photos/IMG_5060.jpeg" alt="DoomCube-2 enclosed printer, viewed from the front" width="600">

**Print time:** 3,746 hours on the mechanical hour counter.

Currently not working: the hotend heater seems to drop out intermittently. I haven’t diagnosed the cause.

## Build and modifications

| Component | Hardware | Reference |
| --- | --- | --- |
| Base printer | Voron 2.4 | [Voron 2.4](https://github.com/VoronDesign/Voron-2) |
| Rebuild | DoomCube-2 | [DoomCube-2 project](https://github.com/FrankenVoron/DoomCube-2) |
| Main controller | FYSETC Spider v2 PCB | [FYSETC Spider project](https://github.com/FYSETC/FYSETC-SPIDER) |
| Firmware | Danger Klipper (now Kalico), commit `e449f3f41055834aafedc4687293ba7ad472fdb1` | [Pinned firmware source](https://github.com/KalicoCrew/kalico/tree/e449f3f41055834aafedc4687293ba7ad472fdb1) |
| Toolhead board | Voron Afterburner Toolhead PCB — Complete — V3.rabbit — ERCF | [Board listing](https://kb-3d.com/store/electronics/357-voron-afterburner-toolhead-pcb-complete-v3rabbit-ercf-1634426646789.html) · [Afterburner PCB project](https://github.com/VoronDesign/Voron-Hardware/tree/master/Afterburner_Toolhead_PCB) |
| Magnetic Z probe | Annex Engineering magnetic probe (likely Quickdraw) | [Quickdraw probe](https://github.com/Annex-Engineering/Quickdraw_Probe) |
| Z endstop | SexBolt Z endstop by hartk1213 | [Design, STL files, and BOM](https://github.com/hartk1213/MISC/tree/main/Voron%20Mods/Voron%202-Trident/2.4/Voron2.4_SexBolt_ZEndstop) · [Assembly manual](https://instructions.online/?id=2461-sexbolt_endstop) |
| Automatic Z calibration | Configured with `[z_calibration]` and `CALIBRATE_Z` on Danger Klipper / Kalico | [Automatic Z-calibration plugin for Klipper](https://github.com/protoloft/klipper_z_calibration) |
| Hour counter | Custom mechanical counter; recorded reading of 3,746 print hours | |
| Expansion PCB | Voron expansion PCB | [Klipper Expander reference](https://github.com/VoronDesign/Voron-Hardware/tree/master/Klipper_Expander) |
| Enclosure lighting | LED lights | |
| Enclosure camera | Camera inside the enclosure | |
| Nozzle cleaning | Toolhead brush | |
| Bed fans | Custom | |
| Air filter | Nevermore carbon air filter | [Nevermore Micro project](https://github.com/nevermore3d/Nevermore_Micro) |

## Photos

[Photos of the build and components](photos/README.md).

## Configuration

[My configuration](config/), including [printer.cfg](config/printer.cfg), probe docking macros in [quickdraw_probe.cfg](config/quickdraw_probe.cfg), and a `[z_calibration]` section in [customize.cfg](config/customize.cfg).

`config/fluidd.cfg` points to `/home/ctso/fluidd-config/client.cfg` on the printer. That file isn’t included here.

I’m running Danger Klipper, now called Kalico, at commit [`e449f3f41055834aafedc4687293ba7ad472fdb1`](https://github.com/KalicoCrew/kalico/tree/e449f3f41055834aafedc4687293ba7ad472fdb1).
