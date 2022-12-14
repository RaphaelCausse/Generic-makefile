[![OS](https://img.shields.io/badge/os-linux-blue.svg)](https://shields.io/)
[![Status](https://img.shields.io/badge/status-completed-success.svg)](https://shields.io/)

# GENERIC MAKEFILE

Generic Makefile for small to medium sized C/C++ projects (OS Linux only).

The Makefile assumes source code is broken up in two groups, header files (.h/.hpp) and implementation files (.c/.cpp).

You can build the project in two modes: Release or Debug.

By default, the build is in Release mode.

<br>

# Table of Contents
 
- [Project Directory Layout](#project-directory-layout)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)

<br>

## PROJECT DIRECTORY LAYOUT

To use this generic makefile properly, please follow this project directory layout.
```
──┬─[ Project ]
  │
  ├──── Makefile
  ├──── README.md
  ├──── LICENSE.md
  │
  │
  ├──┬─[ include ]
  │  └──── *.h / *.hpp
  │
  │
  ├──┬─[ src ]
  │  ├──── main.c / main.cpp
  │  ├──── *.c / *.cpp
  │  ├──┬─[ modules ]
  │  │  └──── *.c / *.cpp
  │  ...
  │
  │
  ...
```
<br>

## INSTALLATION

**Clone** this repository:
```
git clone https://github.com/RaphaelCausse/Generic-makefile.git
```
**Move** to the cloned directory :
```
cd Generic-makefile
```
**Copy** the Makefile in your project.

<br>

## USAGE

**Build** the project (default is Release mode):
```bash
make
make all
make release
```
**Build** the project in Debug mode:
```bash
make debug
```
**Run** the target (default is Release target) :
```
make run
```
or **run** the Debug target:
```bash
make rundbg
```

<br>

## FEATURES

**Clean** the project directory :
```bash
make clean
```
**Display** info about files in project directory:
```bash
make info
```
**Display** help message:
```bash
make help
```
<br>

## AUTHOR

Raphael CAUSSE, 08/2022.

Developped on Manjaro Linux, Visual Studio Code.