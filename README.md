This is a port of many Plan 9 libraries and programs to Unix.

Fork Changes
------------

Compared to the original plan9port this fork contains the following
(notable [there may be others]) differences:

- acme may write a command history to a file (-H option)
- stats can be told to hide machine names (-H option)
- 9front paint was ported (PR for original p9p, so might make it upstream)
- acme: dotfiles are hidden by default and can be toggled with **Dotfiles**
- acme: scratch area contains **Clear** to instantly remove all text
- page: added zoom out
- fix build on Alpine Linux (musl libc)
  - now probably breaking on other linux distributions
    TODO: test and fix (at least for Debian)
- acme: navigation mode for easily travelling through file hierarchy
 
Installation
------------

To install, run ./INSTALL.  It builds mk and then uses mk to
run the rest of the installation.  

For more details, see install(1), at install.txt in this directory
and at https://9fans.github.io/plan9port/man/man1/install.html.

Documentation
-------------

See https://9fans.github.io/plan9port/man/ for more documentation.
(Documentation is also in this tree, but you need to run
a successful install first.  After that, "9 man 1 intro".)

Intro(1) contains a list of man pages that describe new features
or differences from Plan 9.

Helping out
-----------

If you'd like to help out, great!  The TODO file contains a small list.

If you port this code to other architectures, please share your changes
so others can benefit.

Git
---

You can use Git to keep your local copy up-to-date as we make 
changes and fix bugs.  See the git(1) man page here ("9 man git")
for details on using Git.

Status
------

[![Build Status](https://travis-ci.org/9fans/plan9port.svg?branch=master)](https://travis-ci.org/9fans/plan9port)
[![Coverity Scan Build Status](https://scan.coverity.com/projects/plan-9-from-user-space/badge.svg)](https://scan.coverity.com/projects/plan-9-from-user-space)


Contact
-------

* Mailing list: https://groups.google.com/group/plan9port-dev
* Issue tracker: https://github.com/9fans/plan9port/issues
* Submitting changes: https://github.com/9fans/plan9port/pulls

* Russ Cox <rsc@swtch.com>
