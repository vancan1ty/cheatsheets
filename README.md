Cheatsheet Starter -- Currell Berry -- 2/3/2016
===============================================

**Make sure you clone with the --recursive flag!!**

This repository contains a starter quick-reference sheet, which is intended to be used as the basis for various cheatsheets in the future.  This cheatsheet repository/system is based on the late Steve Seiden's "Theoretical Computer Science" cheatsheet.

This repository includes as a submodule the "cheatsheet\_core" repository. In order for the code in this repository to work, you must have initialized the submodule cheatsheet\_core.  The easiest way to do this is to clone the repository with the --recursive flag, like so.

    git clone --recursive [URL-OF-REPO]

Setup Steps
-----------------------------------------------
Currently the Makefile is lightly windows dependent, though it could be switched to fully on unix/linux by changing a few lines.

### setup steps on Windows.
- Download and install Miktex, with standard packages.
- Download and install Cygwin.
- Download and install "poppler" under cygwin.
    - poppler enables pdf merging to create multipage cheatsheets

Once you have done the above install steps, generate output/cheat.pdf with the following command.

    make

See the Makefile for options and flags.

### Linux/Unix
On Unix-like OSes, you should be able to get by with a tex distribution and poppler. You will have to change a few lines in the Makefile.

