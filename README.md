# TerasologyInstallers
This repository contains installers for various different Linux distributions to install Terasology.

All the distributions tested were at their latest versions (or close enough) inside a fresh virtual machine.

# Packages:
  * .deb
  * .rpm
  * .snap

## .deb:  
### Tested Distributions:
* Ubuntu 16.10
* Debian (the original) GNU/Linux 8 (jessie)
 * Notes:
 The GNOME desktop enviroment was used but due to missing dependencies (debian does not yet have openjdk-8) you must install the package by using ` dpkg --install --ignore-depends openjdk-8-jre --ignore-depends openjfx "terasology-launcher_3.1.0-1_all.deb"
 ` in the directory of the package file. To then run the launcher, you must install java-8 manually as well as javafx.

### Notes:
 The package installs to a folder called Terasology Launcher under the main drive (root directory?).
 
## .rpm:
### Tested Distributions:
* Fedora (Does not currently work but the package was built on Fedora)
* OpenSUSE (It works but the bin directory is missing):
 * Notes: Once again the choice of desktop enviroment was GNOME.

### Notes:
 The package installs to usr/bin/terasology-launcher-3.10 but has a missing bin directory. To start the launcher you will have to  launch the Terasology.jar file in the libs folder manually.

## .snap
### Tested Distributions:
* OpenSUSE (broken)
 * Notes: This is currently not working as with snap packages in general (the operating system supports them supposedly)
* Ubuntu 16.10

### Notes:
 Ubuntu generated and installed the packages perfectly but is also the only one to support them in a stable release. OpenSUSE had a broken snap command-line interface when I tried it and Fedora refuses to install the programs needed to use snap packages. Debain's latest weekly build is required supposedly for snap files but for me the build refused to boot properly.
