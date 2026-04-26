# Project README

## Overview
This project is a simple command-line application written in C that demonstrates parsing command-line arguments using a custom CLI library (`CLIArgs`). The application supports various options and can be compiled for different target platforms.

## Features
- Parsing of command-line arguments.
- Support for string, integer, and flag-based options.
- Printing of parsed options.
- Version and help flags.
- Handling of multiple occurrences of the same option.
- Customizable CLI library with support for different data types.

## Project Structure
```
Cmd_CLIArgs/
├── build/              # .exe files produced by Main.c
├── src/                # Source code
│   ├── Main.c          # Entry point
│   └── CLIArgs.h       # Header file for the custom CLI library
├── Makefile.linux      # Linux Build configuration
├── Makefile.windows    # Windows Build configuration
├── Makefile.wine       # Wine Build configuration
├── Makefile.web        # Emscripten Build configuration
└── README.md           # This file
└── LICENSE             # License information
```

### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed in specific projects (example given WINAPI, X11, ALSA)

## Build & Run
- **Linux**:
  ```sh
  cd Cmd_CLIArgs
  make -f Makefile.linux all
  make -f Makefile.linux exe
  ```

- **Windows**:
  ```sh
  cd Cmd_CLIArgs
  make -f Makefile.windows all
  make -f Makefile.windows exe
  ```

- **Wine**:
  ```sh
  cd Cmd_CLIArgs
  make -f Makefile.wine all
  make -f Makefile.wine exe
  ```

- **WebAssembly**:
  ```sh
  cd Cmd_CLIArgs
  make -f Makefile.web all
  make -f Makefile.web exe
  ```

This README provides a clear and concise overview of the project, its features, and how to build and run it on different platforms.