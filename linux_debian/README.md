Creation of a Debian Package

**Currently (v5.0.0 onwards), creation of a Debian package is broken for openNDS.
**

To compile and install openNDS in place, please see the linux_generic README file.

The instructions following are from the original README.md

To create a Debian package of openNDS (a \*.deb file),
you first need to have installed the following programs and libraries:

```
apt install build-essential debhelper devscripts
apt install libmicrohttpd-dev dh-systemd
```

Run this command in the repository root folder to create the package:

```
dpkg-buildpackage
```

The package will be created in the parent directory.


Use this command if you want to create an unsigned package:

```
dpkg-buildpackage -b -rfakeroot -us -uc
```
