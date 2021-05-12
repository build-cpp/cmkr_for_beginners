# cmkr_for_beginners

Try in your browser: [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/build-cpp/cmkr_for_beginners)

Repository for beginners to get started developing C++ with [cmkr](https://github.com/build-cpp/cmkr).

## Building (IDE)

Clone this repository and open it in your favorite IDE with CMake support (Visual Studio, CLion, Qt Creator). Everything should work out of the box.

## Building (command line)

```
cmake -B build
cmake --build build
```

Then open the `.sln` (Windows) or run `make` (Unix) from the `build` directory.

## cmake.toml

Under the hood cmkr generates the `CMakeLists.txt` required to build this project from the `cmake.toml` file:

```toml
[project]
name = "cmkr_for_beginners"
description = "A minimal cmkr project."

[target.example]
type = "executable"
sources = ["src/main.cpp"]
```
