Gforth is a fast and portable implementation of the ANS Forth
language. It works nicely with the Emacs editor, offers some nice
features such as input completion and history, backtraces, a
decompiler and a powerful locals facility, and it even has a
manual. Gforth combines traditional implementation techniques with
newer techniques for portability and performance: its inner
interpreter is direct threaded with several optimizations, but you can
also use a traditional-style indirect threaded interpreter.  Gforth is
distributed under the GNU General Public license (see COPYING).

Gforth runs under GNU, BSD, and similar systems, MS Windows, MacOS X,
OS/2, and DOS and should not be hard to port to other systems
supported by GCC. This version has been tested successfully on the
following platforms:

alpha-unknown-linux-gnu 
 gcc-2.95.2 19991024 (release)
 gcc-2.95.4 20011002 (Debian prerelease) 
 gcc-3.3.6 (Debian 1:3.3.6-15) 
 gcc-3.4.6 (Debian 3.4.6-5) 
 gcc-4.1.2 20061115 (prerelease) (Debian 4.1.1-21)
armv5l-unknown-linux-gnu 
 gcc-3.3.6 (Debian 1:3.3.6-15)
 broken: gcc-4.1.2 20061115 (prerelease) (Debian 4.1.1-21)
           <http://gcc.gnu.org/bugzilla/show_bug.cgi?id=31152>
i686-pc-linux-gnu 
 gcc-2.95.4 20011002 (Debian prerelease) 
 gcc-3.3.5 (Debian 1:3.3.5-13) 
 gcc-3.4.4 20050314 (prerelease) (Debian 3.4.3-13sarge1)
ia64-hp-hpux11.23 
 gcc-4.1.1
 broken: gcc-3.4.3
powerpc-unknown-linux-gnu 
 gcc-2.95.4 20011002 (Debian prerelease) 
 gcc-3.2.3 (Debian) 
 gcc-3.3.6 (Debian 1:3.3.6-15) 
 gcc-3.4.6 (Debian 3.4.6-8) 
 gcc-4.0.3 20060128 (prerelease) (Debian 4.0.2-8) 
 gcc-4.1.3 20080623 (prerelease) (Debian 4.1.2-23) 
 gcc-4.3.2
powerpc64-unknown-linux-gnu 
 gcc-3.4.6 (Debian 3.4.6-5) 
 gcc-4.1.2 20061115 (prerelease) (Debian 4.1.1-21)
sparc-sun-solaris2.10 
 gcc-3.4.3 (csl-sol210-3_4-branch+sol_rpath) 
 gcc-4.0.2
x86_64-unknown-linux-gnu 
 gcc-3.3.6 (Debian 1:3.3.6-15) 
 gcc-3.4.6 (Debian 3.4.6-5) 
 gcc-4.0.0
 gcc-4.0.4 20060904 (prerelease) (Debian 4.0.3-7) 
 gcc-4.1.2 20061115 (prerelease) (Debian 4.1.1-21)
 gcc-4.1.3 20080623 (prerelease) (Debian 4.1.2-23) 
 gcc-4.2.0
 gcc-4.2.4 (Debian 4.2.4-3) 
 gcc-4.3.1
i386-apple-darwin9.4.0
x86_64-apple-darwin9.4.0
ppc-apple-darwin9.4.0
i686-pc-cygwin
gforth-ec: r8c, 4stack, misc, 8086

Read INSTALL for installation instructions from source, or INSTALL.DOS
for DOS, Windows, and OS/2 from source, or INSTALL.BINDIST if you have
a binary package distributed as .tar.gz or .zip file.  If you received
a self-installing executable, just run it and follow the instructions.

To start the system, just say `gforth' (after installing it).

You can find new versions of Gforth at ftp://ftp.gnu.org/gnu/gforth/
and its mirrors or at

http://www.complang.tuwien.ac.at/forth/gforth/
or
ftp://ftp.complang.tuwien.ac.at/pub/forth/gforth/

The latter site also contains binary distributions of Gforth for some
popular platforms.

If you want to work on Gforth, mail me. Tasks to be done can be found
in ToDo; but if you would like to do something not mentioned there,
it's ok, too. In any case, we would like to hear what you are
doing. The most important task IMO is the foreign language interface
for C.

On popular request, here are the meanings of unusual file extensions:

*.fs	Forth stream source file (include with "include <file>" from within
        gforth, or start with "gforth <file1> <file2> ...")
*.fi	Forth image files (start with "gforth -i <image file>")
*.fb	Forth blocks file (load with "use <block file> 1 load")
*.i	C include files
*.ds	documenation source
*TAGS	etags files

A number of Forth source files are included in this package that are
not necessary for building Gforth. Not all of them are mentioned in
the rest of the documentation, so here's a short overview:

Add-ons:
code.fs random.fs more.fs ansi.fs colorize.fs
oof.fs oofsampl.fs objects.fs blocked.fb tasker.fs

Utilities:
ans-report.fs etags.fs glosgen.fs filedump.fs

Games:
tt.fs sokoban.fs

Test programs (for testing Forth systems):
test/*.fs

Benchmarks:
bubble.fs siev.fs matrix.fs fib.fs

ANS Forth implementations of Gforth extensions:
compat/*.fs

For discussions about Gforth, use the Usenet newsgroup
comp.lang.forth.  If you prefer not to post on Usenet, there is also a
mailing list: GForth@ChaosSolutions.org.  To subscribe, send a mail to
gforth-subscribe@chaossolutions.org with:

subscribe GForth

as the first and only line within the message body.  You can also
report bugs through these channels, or you can report them through our
bug database:

https://savannah.gnu.org/bugs/?func=addbug&group=gforth

- anton
anton@mips.complang.tuwien.ac.at
http://www.complang.tuwien.ac.at/anton/home.html
-----
Copyright (C) 1995,1996,1997,1998,2000,2003,2004,2006,2007,2008 Free Software Foundation, Inc.

This file is part of Gforth.

Gforth is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation, either version 3
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.#See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see http://www.gnu.org/licenses/.
