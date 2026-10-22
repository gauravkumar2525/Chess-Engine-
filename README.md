# RookForge — C++ Chess Engine Study

RookForge is a renamed working copy for studying and extending a C++ chess engine with a UCI interface and an optional GTK4 graphical interface.

**Attribution:** This code is derived from the upstream `chess_engine` project.

Before redistributing or publishing this code publicly, verify the upstream repository's licensing terms and obtain permission if required. The supplied archive did not include a clear open-source `LICENSE` file, so public redistribution rights are not established by this ZIP alone.

## Features described by the upstream project

- C++ chess engine with a UCI interface
- Minimax search with alpha-beta pruning
- Quiescence search and iterative deepening
- Move-ordering and evaluation heuristics
- Perft and EPD-based test fixtures
- Optional GTK4 graphical interface

These are inherited project features; verify them against the source and tests before making performance or correctness claims.

## Requirements

- CMake 3.20 or newer
- A C++23-compatible compiler
- GTK4 and `pkg-config` for the optional GUI target

## Build with CMake

```bash
cmake -B build -S . -DCMAKE_BUILD_TYPE=Debug
cmake --build build
```

The GUI target is optional and depends on GTK4 being available. If the configuration does not find GTK4, the GUI may not be built.

## Build with Make

On Linux, if the required dependencies are installed:

```bash
cd src
make
./main
```

Check the Makefile for the exact targets available in your environment.

## Tests

Test assets and scripts are in `tests/`. Review their dependencies and run them in the target environment. Build and test status should be documented only after running the commands successfully.

## Making this your own

For a portfolio project, document your own original work separately: features you implemented, bugs you fixed, tests you added, design decisions, and benchmark results. Keep upstream attribution and all applicable license notices intact.
