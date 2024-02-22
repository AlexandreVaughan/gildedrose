# Gilded Rose refactoring kata (C++)

## Introduction

This is a C++ version of the GildedRose refactoring Kata using the [Googletest](https://github.com/google/googletest) test framework in the `test/cpp_googletest_unittest` folder.

There is also a standard (command line) test in the `test/cpp_text_test` folder.

The kata was slightly modified to add a dependency to a *status bar* which should also be refactored. (See GildedRoseRequirements.md).

## Prerequisites

* CMake version >= 3.13
* C++ compiler that support C++11

## How to build and run tests in a terminal

### Build tests

    $ cd ${GIT_FOLDER}/GildedRose-Refactoring-Kata/cpp
    $ mkdir build
    $ cd build
    $ cmake ..
    $ cmake --build .

### Show available tests

    $ cd ${GIT_FOLDER}/GildedRose-Refactoring-Kata/cpp/build
    $ ctest -N
    Test project ${GIT_FOLDER}/GildedRose-Refactoring-Kata/cpp/build
      Test #1: GildedRoseGoogletestUnitTests
      Test #2: GildedRoseTextTests

### Run all tests

    $ ctest -C Debug

### Run all tests with verbose output

    $ ctest -C Debug -VV

## How to build and run tests using Visual Studio 2019 

1. Start Visual Studio 2019
2. Select `Open a local folder`
3. Select folder `${GIT_FOLDER}/GildedRose-Refactoring-Kata/cpp`
4. Wait for message `CMake generation finished.` in the CMake output window at the bottom
5. Select what test variant to run in the drop down menu for Startup Items, e.g. `GildedRoseGoogletestUnitTests.exe`.
6. Select menu `Debug - Start`
