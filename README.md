# MXE (M cross environment)

[![Travis build][travis-badge]][travis-page]
[![License][license-badge]][license-page]

[travis-page]: https://travis-ci.org/mxe/mxe
[travis-badge]: https://travis-ci.org/mxe/mxe.png
[license-page]: LICENSE
[license-badge]: http://img.shields.io/badge/License-MIT-brightgreen.png

MXE (M cross environment) is a Makefile that compiles a cross
compiler and cross compiles many free libraries such as SDL and
Qt. Thus, it provides a nice cross compiling environment for
various target platforms, which:

  * is designed to run on any Unix system
  * is easy to adapt and to extend
  * builds many free libraries in addition to the cross compiler
  * can also build just a subset of the packages, and automatically builds their dependencies
  * downloads all needed packages and verifies them by their checksums
  * is able to update the version numbers of all packages automatically
  * directly uses source packages, thus ensuring the whole build mechanism is transparent
  * allows inter-package and intra-package parallel builds whenever possible
  * integrates well with autotools, cmake, qmake, and hand-written makefiles.
  * has been in continuous development since 2007 and is used by several projects

## Supported Toolchains

  * Runtime: MinGW-w64
  * Host Triplet:
    - `i686-w64-mingw32`
    - `x86_64-w64-mingw32`
  * Packages:
    - static
    - shared

Shared support in MXE was just added in early February, 2014.
