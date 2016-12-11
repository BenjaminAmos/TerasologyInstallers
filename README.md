# TerasologyInstallers
This repository contains installers for various different Linux distributions to install Terasology.

All the distributions tested were at their latest versions (or close enough).

# Packages:
  * .deb
  * .rpm

## .deb:  
### Tested Distributions:
* Ubuntu
* Debian (the original)
 * Notes:
 The GNOME desktop enviroment was used but the package manager installed it perfectly so any GUI could work potentially.

### Notes:
 The package installs to a folder called Terasology Launcher under the main drive (root directory?).
 
## .rpm:
### Tested Distributions:
* Fedora (Does not currently work but the package was built on Fedora)
* OpenSUSE (It works but the bin directory is missing):
 * Notes: Once again the choice of desktop enviroment was GNOME.

### Notes:
 The package installs to usr/bin/terasology-launcher-3.10 but has a missing bin directory. To start the launcher you will have to  launch the Terasology.jar file in the libs folder manually.
