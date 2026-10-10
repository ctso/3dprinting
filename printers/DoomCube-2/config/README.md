# DoomCube-2 configuration

The supplied configuration backup is stored in [config.tgz](config.tgz). It contains the original `config/` directory, including Klipper configuration, macros, Moonraker configuration, Crowsnest configuration, and a hidden Moonraker backup.

The Home Assistant `token` values in `config/moonraker.conf` and `config/.moonraker.conf.bkp` were replaced with `REDACTED`. All other file contents and archive entries were preserved. The archive was repacked to apply those redactions.

The backup includes machine-specific paths, private network addresses, and MCU serial identifiers. Its `config/fluidd.cfg` entry is an absolute symlink to `/home/ctso/fluidd-config/client.cfg`; the linked file's contents are not included. Restoring the Home Assistant integration requires supplying a token locally.

`quickdraw_probe.cfg` contains probe docking macros, and `customize.cfg` contains a `[z_calibration]` section.

The owner reports that this printer runs Danger Klipper (now Kalico) at commit [`e449f3f41055834aafedc4687293ba7ad472fdb1`](https://github.com/KalicoCrew/kalico/tree/e449f3f41055834aafedc4687293ba7ad472fdb1). This firmware reference was supplied separately from the backup. The source of the installed Z-calibration module remains to be confirmed.
