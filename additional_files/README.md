<!--
This file serves as an example for a readme file in Nostra Projects, it is NOT the readme file for this (the Nostra 
conventions) project.
-->

# NostraTestProject

An exemplary project that is part of Nostra.

GitHub: &lt;the link to GitHub would go here, but this example has no GitHub repository&gt;

To clone the repository to your local machine, use the command
```
git clone <still no link>
```
Alternatively, it is possible to download the repository as a ZIP archive from GitHub using the link above.

## Requirements
### Usage Requirements
To use the library, a C++ compiler is required that supports the C++17 standard.

### Build Requirements
To build only the library, a C++ compiler that supports the C++17 standard and the CMake (https://www.cmake.org/) build 
system are required. Additionally, __make__ is required on Linux, __XCode__ is required on MacOs and __Visual Studio__
is required on Windows.

To also build the documentation of the project, Doxygen (http://www.doxygen.nl/) is required.

# How to build
First of all, the following steps assume that the current working directory of the shell is the root directory of the 
project (the one that the file __CMakeLists.txt__ is in). It is also assumed that the command __cmake__ is in the PATH
variable.

The single steps in the build process are:
1. ```mkdir build```
2. ```cd build```
3. ```cmake ..```
4. ```cmake --build .```

It is also possible to pass various variables to the third command. These have the syntax
```-D<variable name>=<value>```
The following list describes some of the most commonly used variables.

* CMAKE_INSTALL_PREFIX: The value is the path to the directory that the library should later be installed in. The
  default value varies from system to system.
* BUILD_TESTING: The value is either ON or OFF. It determines weather the tests should be build or not. The default 
  value is ON.
* NOSTRA_BUILD_EXAMPLES: The value is either ON or OFF. It determines weather the examples should be build or not. The 
  default value is ON.
* NTP_BUILD_DOC: The value is either ON or OFF. It determines weather the documentation will be build or not. The 
  default value is ON.

# How to install
If the project was build from source, the command
```cmake --build . --target install```
will install the project.

Currently, there is no other option and no installer is provided.

## Changelog
### Version 1.1.0.0
#### Additions
* Added component new_feature_in_one_point_one
#### Removals
* None
#### Deprecations
* bad_feature is now marked as deprecated
#### Improvements
* slow_feature's overall performance has been improved
#### Fixes
* buggy_feature::set_value() now sets the value correctly
#### Known Issues
* buggy_feature::get_value() does not return the correct value

### Version 1.0.0.0
#### Additions
* Added component slow_feature
* Added component buggy_feature
* added component new_feature 
#### Removals
* None
#### Deprecations
* None
#### Improvements
* None
#### Fixes
* None
#### Known Issues
* buggy_feature::set_value() does not set the correct value
* buggy_feature::get_value() does not return the correct value

