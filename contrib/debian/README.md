
Debian
====================
This directory contains files used to package dashblackd/dashblack-qt
for Debian-based Linux systems. If you compile dashblackd/dashblack-qt yourself, there are some useful files here.

## dashblack: URI support ##


dashblack-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install dashblack-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your dashblackqt binary to `/usr/bin`
and the `../../share/pixmaps/dashblack128.png` to `/usr/share/pixmaps`

dashblack-qt.protocol (KDE)

