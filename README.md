# ThinkPad ACPI backlight management

Basic ACPI actions to control the backlight of some recent ThinkPad (T470).
Based on [acpilight](https://github.com/wavexx/acpilight) udev script and
xbacklight replacement.

## Usage
Just install it (`makepkg` and `pacman -U tpacpi-backlight....pkg.tar.xz`) and restart the `acpid`
service (of course, it must be enable to have backlight keys working at startup).

## Notes
This is a simple WiP mainly for myself.

The udev script is useless for the ACPI actions, but allow to use xbacklight manually by
being in `video` group.
It should be fixed in the AUR of `acpilight` and not there.

However, I hope to extand it later.
And I hope this small example can be useful for other people ;)
