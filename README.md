sj
==

"Platform independent" co-routine library exposed through a minimal C API.
Future plans also include a type-safe C++ API.

I say "platform independent" since it *technically* supports a heap of
different platforms, but the projects are not yet set up to support them. The
only currently supported project configuration is for VS2015 (possibly 2013,
I haven't tested yet).

Uses assembly from [boost::context] to do the heavy lifting.

Building
--------

Project generation is done through [GENie].

1. Download [GENie].
2. Run `genie <action>` in the root folder to generate project files. Refer to
   `genie --help` for the different actions (project types).
3. Open up the **build** folder and build the projects.

To run the tests, build and run the **sj_tests** project.

License
-------

Copyright (c) 2016, Johan Sköld

Permission to use, copy, modify, and/or distribute this software for any  
purpose with or without fee is hereby granted, provided that the above  
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES  
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF  
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR  
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES  
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN  
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF  
OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.

[GENie]:            https://github.com/bkaradzic/GENie      "bkaradzic/GENie"
[boost::context]:   https://github.com/boostorg/context     "boostorg/context"
