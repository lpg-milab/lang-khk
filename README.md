The Halh (Khalkha) Mongolian morphology and tools
==========================================

[![GitHub issues](https://img.shields.io/github/issues-raw/giellalt/lang-khk)](https://github.com/giellalt/lang-khk/issues)
[![Build Status](https://github.com/giellalt/lang-khk/workflows/Speller%20CI+CD/badge.svg)](https://github.com/giellalt/lang-khk/actions)
[![License](https://img.shields.io/github/license/giellalt/lang-khk)](https://github.com/giellalt/lang-khk/blob/main/LICENSE)

This repository contains finite state source files for the Halh Mongolian language,
for building morphological analysers, proofing tools
and dictionaries. The data and implementation are licenced under __LICENSE__
licence, also detailed in the
[LICENSE](https://github.com/giellalt/lang-khk/blob/main/LICENSE). The
authors named in the AUTHORS file are available to grant other licencing
choices.

Install proofing tools and [keyboards](https://github.com/giellalt/keyboard-khk)
for the Halh Mongolian language by using the [Divvun Installer](http://divvun.no)
(some languages are only available via the nightly channel).

Documentation
-------------

Documentation can be found at:

-   <https://giellalt.uit.no/lang/khk/KhalkhaMongolianDocumentation.html>
-   <https://giellalt.uit.no/index.html>

Core dependencies
-----------------

In order to compile and use Halh Mongolian language morphology and
dictionaries, you need:

- an FST compiler: [HFST](https://github.com/hfst/hfst), [Foma](https://github.com/mhulden/foma) or [Xerox Xfst](https://web.stanford.edu/~laurik/fsmbook/home.html)
- [VislCG3](https://visl.sdu.dk/svn/visl/tools/vislcg3/trunk) Constraint Grammar tools

To install VislCG3 and HFST, just copy/paste this into your Terminal on **Mac OS X**:

```
curl https://apertium.projectjj.com/osx/install-nightly.sh | sudo bash
```

or terminal on **Ubuntu, Debian or Windows Subsystem for Linux**:

```
wget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash
sudo apt-get install cg3 hfst
```

or terminal on **RedHat, Fedora, CentOS or Windows Subsystem for Linux**:

```
wget https://apertium.projectjj.com/rpm/install-nightly.sh -O - | sudo bash
sudo dnf install cg3 hfst
```

Alternatively, the Apertium wiki has good instructions on how to [install the dependencies for Mac
OS X](https://wiki.apertium.org/wiki/Apertium_on_Mac_OS_X) and how to [install
the dependencies on
linux](https://wiki.apertium.org/wiki/Installation_of_grammar_libraries)

Further details and dependencies are described on the GiellaLT [Getting Started](https://giellalt.uit.no/infra/GettingStarted.html) pages.

Downloading
-----------

Using Git:
```
git clone https://github.com/giellalt/lang-khk
```

Using Subversion:
```
svn checkout https://github.com/giellalt/lang-khk.git/trunk lang-khk
```

Building and installation
-------------------------

[INSTALL](https://github.com/giellalt/lang-khk/blob/main/INSTALL)
describes the GNU build system in detail, but for most users it is the usual:

```sh
./autogen.sh # This will automatically clone or check out other GiellaLT dependencies
./configure
make
(as root) make install
```
