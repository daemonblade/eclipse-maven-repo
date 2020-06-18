# Offline Maven Repository for FreeBSD Eclipse

This project contains maven dependencies required to build
FreeBSD's [/usr/ports/java/eclipse](https://svnweb.freebsd.org/ports/head/java/eclipse/).

It also acts as an alternate MASTER_SITE for Eclipse build
sources, as git.eclipse.org can be quite erratic.

## Layout

* **README.md** This file
* **p2-stub** Contains stub files for offline build.
* Everything else are files fetched from a full online build.

## Refreshing the Project

1. Requires a working build of
[freebsd-eclipse](https://github.com/daemonblade/freebsd-eclipse).
1. Remove all files (including `.cache` and `.meta`) except for
`README.md` and `p2-stub`.
1. Copy the contents of `freebsd-eclipse/maven-repo.${VERSION}`
to the project.

## Releases

1. Commit and tag for release to match java/eclipse PORTVERSION
1. Add Eclipse source tarballs to the release
