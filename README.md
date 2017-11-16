UTPP - A New Generation of UnitTest++
=====================================

This test library is based on UnitTest++. See below for README notes of UnitTest++.

Latest version can be downloaded from [GitHub](https://neacsum.github.com/utpp) or
[BitBucket](https://bitbucket.org/neacsum/utpp).

There is also [documentation](https://neacsum.github.io/utpp) generated with Doxygen.


Author:
Mircea Neacsu (mircea@neacsu.net)

See architecture.md file for details

## License ##

The MIT License (MIT)
 
Copyright (c) 1999-2017 Mircea Neacsu

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


## UnitTest++ README ##
Version: v1.4
Last update: 2008-10-30

UnitTest++ is free software. You may copy, distribute, and modify it under
the terms of the License contained in the file COPYING distributed
with this package. This license is the same as the MIT/X Consortium
license.

See src/tests/TestUnitTest++.cpp for usage.

Authors:
Noel Llopis (llopis@convexhull.com) 
Charles Nicholson (charles.nicholson@gmail.com)

Contributors:
Jim Tilander
Kim Grasman
Jonathan Jansson
Dirck Blaskey
Rory Driscoll
Dan Lind
Matt Kimmel -- Submitted with permission from Blue Fang Games
Anthony Moralez
Jeff Dixon
Randy Coulman
Lieven van der Heide

Release notes:
--------------
Version 1.4 (2008-10-30)
- CHECK macros work at arbitrary stack depth from inside TESTs.
- Remove obsolete TEST_UTILITY macros
- Predicated test execution (via TestRunner::RunTestsIf)
- Better exception handling for fixture ctors/dtors.
- VC6/7/8/9 support

Version 1.3 (2007-4-22)
- Removed dynamic memory allocations (other than streams)
- MinGW support
- Consistent (native) line endings
- Minor bug fixing

Version 1.2 (2006-10-29)
- First pass at documentation.
- More detailed error crash catching in fixtures.
- Standard streams used for printing objects under check. This should allow the
  use of standard class types such as std::string or other custom classes with
  stream operators to ostream.
- Standard streams can be optionally compiled off by defining UNITTEST_USE_CUSTOM_STREAMS
  in Config.h
- Added named test suites
- Added CHECK_ARRAY2D_CLOSE 
- Posix library name is libUnitTest++.a now
- Floating point numbers are postfixed with f in the failure reports

Version 1.1 (2006-04-18)
- CHECK macros do not have side effects even if one of the parameters changes state
- Removed CHECK_ARRAY_EQUAL (too similar to CHECK_ARRAY_CLOSE)
- Added local and global time constraints
- Removed dependencies on strstream
- Improved Posix signal to exception translator
- Failing tests are added to Visual Studio's error list
- Fixed Visual Studio projects to work with spaces in directories

Version 1.0 (2006-03-15)
- Initial release

