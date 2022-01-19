# ZRDX DOS Extender

This repository contains the source code of ZRDX v0.50, released 2000-07, for the purpose of archival and preservation. As of 2022-01, the original host website at [www.zrdx.da.ru](http://www.zrdx.da.ru/) is no longer available, but is archived on the [Wayback Machine](https://web.archive.org/web/20050313054840/http://dx.zr.spb.ru/).

No changes have been made aside from converting all file and directory names  to lowercase, and the addition of this readme. 

ZRDX is Copyright &copy; 1998-1999 by Sergey Belyakov.

## Overview

ZRDX can be used to run programs, designed for DOS4G/W, PMODE/W, DOS32A,
WDOSX via Watcom C++, TMT Pascal, LadSoft C, etc. compilers.

Application running under ZRDX can access all physical memory (up to 4G),
all DPMI functions (int 31h) are compatible with DPMI 0.9 specification,
except fns 0A00h-0B03h. DOS extender provides translation of all functions,
translated by PMODE/W, except identification fns, and almost all functions,
translated by DOS4G/W. If you are using only standard libraries, these fns
are quietly enough for your programs to run. If you call DOS directly, you
may examine the list of all translated functions in file 'src/extender.asm'.

You are encouraged to use UPX for packing your executables. It is much more
effective than PMWLITE or any other executables packer, and supports wide
variety of target platforms.

## License

ZRDX 0.50 is distributed as freeware and can be freely copied and used in
any purposes, either commercial or non-commercial. There are no restrictions
applied to development and use of software which can be created via modifying or extending original ZRDX source files or binary code.

ZRDX is distributed "AS IS". The author does not guarantee fitness for any
particular purpose, and can not be held responsible for any advantages or
misadvantages coming from using or not using this product.

All rights on original source files are reserved by the author, Sergey
Belyakov.

