## pkg-latex-metropolis

_Unofficial_ [Debian](http://www.debian.org) packaging for the 
[Metropolis](https://github.com/matze/mtheme) theme for Beamer presentations

### About

This repository provides a simple way to create a .deb file with the required
style files for [Metropolis](https://github.com/matze/mtheme) (formerly known
as mtheme).

### Installation

#### Local Build

After cloning the repository run

```
dpkg-buildpackage -rfakeroot -us -uc -tc
```

to create a Debian binary using the common _fake_ suid accessor, without
signing changes or control file as we are not uploading anywhere, and
cleaning up.  More easily, just run

```
./runMe.sh
```

and either one of these two will create a `.deb` package containing the
desired fonts.

#### PPA

The package is available pre-built from my
[PPA](https://launchpad.net/~edd/+archive/ubuntu/misc) which can be added to
list of repositories known to `apt` et al the usual way.

### Status

This is a somewhat ad-hoc package for personal use.  It takes a shortcut in
packaging / building. That is not exactly how Debian does things.  But it
provides the lovely [Metropolis](https://github.com/matze/mtheme) and that is
a Good Thing (tm).

### Author

Dirk Eddelbuettel

### License

The packaging is provided under the GPL (version 2 or later).  The underlying
LaTeX files are included unaltered, and licensed under
[CC By-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).
