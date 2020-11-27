
Debian
====================
This directory contains files used to package ggcashd/ggcash-qt
for Debian-based Linux systems. If you compile ggcashd/ggcash-qt yourself, there are some useful files here.

## ggcash: URI support ##


ggcash-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install ggcash-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your ggcash-qt binary to `/usr/bin`
and the `../../share/pixmaps/ggcash128.png` to `/usr/share/pixmaps`

ggcash-qt.protocol (KDE)

