# DoomCube-2 configuration

The supplied configuration backup is stored in [config.tgz](config.tgz). It contains the original `config/` directory, including Klipper configuration, macros, Moonraker configuration, Crowsnest configuration, and a hidden Moonraker backup.

The Home Assistant `[power main]` sections were removed from `config/moonraker.conf` and `config/.moonraker.conf.bkp`, along with the related `POWER_OFF` macro in `config/macros/helpers.cfg` and its idle-timeout call in `config/core_hardware.cfg`. All other file contents and archive entries were preserved. The archive was repacked to apply these changes.

The backup includes machine-specific paths, trusted network ranges, and MCU serial identifiers. Its `config/fluidd.cfg` entry is an absolute symlink to `/home/ctso/fluidd-config/client.cfg`; the linked file's contents are not included.

`quickdraw_probe.cfg` contains probe docking macros, and `customize.cfg` contains a `[z_calibration]` section.

The owner reports that this printer runs Danger Klipper (now Kalico) at commit [`e449f3f41055834aafedc4687293ba7ad472fdb1`](https://github.com/KalicoCrew/kalico/tree/e449f3f41055834aafedc4687293ba7ad472fdb1). This firmware reference was supplied separately from the backup. The source of the installed Z-calibration module remains to be confirmed.
