pthread.h
=========

This is a pthreads wrapper originally found at [wiibrew][1]. It only provides
basic pthread functionality and uses libogc's liwghtweight processes (LWP)
internally. Support for conditional variables is currently missing, but
could be added later, as LWP supports them.

[1]: http://wiibrew.org/wiki/Pthread


Installation
------------

You need to add pthread.h to an include folder used when compiling your
game/application. Be careful when adding it to a global include folder
(e.g. libogc/include) as it could interfere with other things. For example
a build system of a portlib could find the header and assume full pthreads
support, which this header file not provides.
