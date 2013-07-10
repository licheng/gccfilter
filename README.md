gccfilter
=========

Introduction
------------

This version of gccfilter is obtained from https://github.com/dichlofos/gccfilter
that is a derived work from Emmanuel Le Trong gccfilter project containing
some bugfixes and improvements.

Description
-----------

Here follows the original description from Emmanuel Le Trong <manu@mixtion.org>.

gccfilter is a perl filter to colorize and simplify (or expand)
gcc diagnostic messages.

gccfilter is particularly aimed at g++ (i.e. dealinging with C++)
messages which can contain lot of template-related errors or warnings
difficult to sort out.

Features:

* coloring of diagnostic messages (with customizable colors),
* simplification of templated programs output: removal of "with" clauses, template arguments,
* inline replacement of template arguments by their values,
* removal of namespaces,
* removal of instantiation chains.

There exists a somewhat similar tool [colorgcc](http://schlueters.de/colorgcc.html).
However it seems to be unmaintained for years now and does only coloring.

Note that the script relies on several perl modules, namely:

* Term::ANSIColor(3perl)
* Getopt::ArgvFile(3pm)
* Getopt::Long(3perl)
* Regexp::Common(3pm)

So far it also requires perl version 5.9.4 or above (for the "state" keyword).
If it's really a problem, let me know, i'll use a closure instead.

Download the script: <http://www.mixtion.org/gccfilter/gccfilter>
and put it somewhere in your $PATH.

The man page is integrated in the file (type gccfilter -m),
or available in HTML here: <http://www.mixtion.org/gccfilter/gccfilter.html>

Author
------
Emmanuel Le Trong, <manu@mixtion.org>
