Octave Patch Queue(s)
=====================

This repository contains my patch queue(s) for works in progress on the
GNU Octave (http://www.octave.org) project.

Instructions
------------

1) Set up an existing patch queue:

  $ cd /path/to/src/octave
  $ hg qqueue -c NAME
  $ cd .hg
  $ git clone -b patches-NAME https://github.com/mtmiller/octave-patch-queue.git  patches-NAME
  $ cd ..
  $ hg qseries

2) Create a new patch queue:

  $ cd /path/to/src/octave
  $ hg qqueue -c NAME
  $ cd .hg
  $ git clone https://github.com/mtmiller/octave-patch-queue.git patches-NAME
  $ cd patches-NAME
  $ git checkout -b patches-NAME
  $ cd ../..
  $ hg qnew foo.diff

License
-------

This set of patches applies only to GNU Octave so they are licensed
under the same terms as GNU Octave itself.

This package is free software: you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by the
Free Software Foundation, either version 3 of the License, or (at your
option) any later version.

This package is distributed in the hope that it will be useful, but
WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the file
COPYING for more details.
