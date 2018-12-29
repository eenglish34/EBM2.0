
Debian
====================
This directory contains files used to package pivxd/ebm-qt
for Debian-based Linux systems. If you compile pivxd/ebm-qt yourself, there are some useful files here.

## pivx: URI support ##


ebm-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install ebm-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your pivxqt binary to `/usr/bin`
and the `../../share/pixmaps/pivx128.png` to `/usr/share/pixmaps`

ebm-qt.protocol (KDE)

