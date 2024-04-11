# C++ project starter

## Introduction

An initial setup of directory structure, CMake, formatting and linting tools and tasks for C++ projects developed using Visual Studio Code (but not exclusively if you just ignore the _.vscode_ dir). The structure features a _src_ directory that is supposed to be split into modules, a _tests_ directory for testing (using _gtest_ by default) and an _app_ directory to store the main-function-like code. It takes advantage of CMake presets and gives an example of a CMake macro definition to fetch libraries directly from a git remote. The project also contains clang-format and clang-tidy configurations, set to Google style with a manual config of naming conventions in the .clang-tidy file.

## Use

### Extensions

It is recommended that you install the recommended extensions when prompted by a VS Code popup. Another way is to manually install the extensions listed in _.vscode/extensions.json_.

### CMake

The easiest way to configure the project is to click the 'Yes' button when prompted by VS Code if you'd like to configure the CMake project. You can change how the presets behave in the _CMakePresets.json_ file. After configuration, you can build the project with provided VS Code tasks or with CMake commands from the terminal.

### Installing requirements - Windows

This project makes use of CMake, LLVM tools, ninja and a C++ compiler. These are recommended to be installed via [_scoop_](https://scoop.sh). Scoop can be installed with a Powershell script (_install-scoop.ps1_) provided in the _scripts_ directory. When scoop is installed, you can install all the necessary packages with the second script - _install-requirements-scoop.ps1_. The compiler of choice in the script is the GNU compiler.

### Installing requirements - Linux

TBD (you can most likely install all of the necessary packages via your package manager, e.g. _apt_, but the versions can be old, which can be detrimental)

## Authors

- Wojciech Przybylski @wprzyby wojciech.przybylski2.stud@pw.edu.pl

