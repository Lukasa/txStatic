txStatic
========

txStatic is a library that provides an extended, more-powerful version of the `File`_ class from Twisted Web. The goal of this module is to prototype more advanced functionality for serving static files with the goal of improving efficiency and providing an experience more like what you'd get from a server like nginx.

txStatic has the following features:

- Last-Modified support (inherited from the implementation in Twisted Web)
- Etag support (using the same etag calculation mechanism as nginx)
- Support for pre-compressing files, and serving compressed versions of a file when appropriate.
- Disables directory lookups.
- Automatic Link header emission based on HTML content.

In the future we'd like txStatic to become a testbed for adding more advanced efficiency tools to Twisted Web, including:

- HTTP/2 server push
- HTTP/2 Cache Digests
- 103 Early Hints responses


Current Status
--------------

Right now txStatic is under active development. Please consider using it, but be aware that it is not necessarily production-ready.


License
-------

txStatic is made available under the MIT license. This module contains code that was originally part of the Twisted project, and that code was also made available under the MIT license. See LICENSE for more details.


.. _File: https://twistedmatrix.com/documents/current/api/twisted.web.static.File.html
