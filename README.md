# Offline Maven Repository for FreeBSD Eclipse

This project contains maven dependencies required to build
FreeBSD's /usr/ports/java/eclipse.

# Layout

* **README.md** This file
* **p2-stub** Stub file for offline build.

## Refreshing the Project

1. Require a working [freebsd-eclipse](https://github.com/daemonblade/freebsd-eclipse)
build.
1. Remove all files except for `README.md` and `p2-stub`; this
includes `.cache` and `.meta`.
1. Copy the contents of `freebsd-eclipse/maven-repo.${VERSION}`
to the project.
1. Commit and tag for release to match java/eclipse PORTVERSION
