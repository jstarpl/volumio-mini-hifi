Volumio Mini HiFi configuration
===

GPIOs
---
For Allo Boss GPIO header pinout see: https://www.audiophonics.fr/img/cms/Images/Produits/12K/12533/gpio-header---inpage2.jpg
The LED light is connected to GPIO27 (Allo Boss GPIO pin 10) and GND.
Button is connected to GPIO17 (Allo Boss GPIO pin 8) and GND.

GPIO17 needs the Pull-up Resistor to be on, as configured in userconfig.txt

Special sauce
---
GPIO-Buttons has a special feature where a long-press of the play/pause button will eject the CD from the drive.

The `/usr/local/bin/autodvd` script along with the *udev* configuration automatically mounts any inserted data disk on `/mnt/CDROM`.
