# Building Setup Packages with the InstallForge CLI Builder

This guide shows how to build your InstallForge setup executables from the command line. It’s aimed at CI/CD pipelines
and automated build scripts as well as local “one-shot” builds.

## Prerequisites

- You have an **InstallForge project file** (e.g. `MyProject.ifp`)
- On CI: use a **Windows runner/agent** (e.g., GitHub Actions `windows-latest`, Azure Pipelines `windows-latest`, GitLab
  Windows runner).

## Locate the CLI

The CLI builder lives in the `bin` folder, which located in the root installation folder of InstallForge.

```bat
REM Typical path on a 64-bit system:
"C:\Program Files (x86)\solicus\InstallForge\bin\ifbuildx86.exe"
```

!!! tip

    It is advised to launch the CLI builder from the InstallForge Shell Environment, which sets up all necessary
    environment variables. The Shell Environment can be launched with the `ifbuild.bat`, which is also located in
    the build folder.

## Quick Start

```bat
REM Typical path on a 64-bit system:
ifbuildx86.exe -i "MyProject.ifp"
```

On success, the CLI returns exit code `0`. Otherwise, `1` is returned.

## Command-Line Interface Reference

```bat
Usage:
  ifbuildx86.exe -i <input.ifp> [-o <output.exe>] [--quiet] [--version] [-h]

Options:
  -i  InstallForge project file path (*.ifp)
  -o  Overwrite setup package executable file path from project file

Global Flags:
     --no-color  Disable console ANSI colors
      --version  Print application version information
  -h, --help     Print this help
```

!!! info

    The CLI builder supports ANSI colors in the console output by default. If your console does not support ANSI
    colors, you can disable them with the `--no-color` flag. Alterntively, you can also set the environment variable
    `NO_COLOR` to any value in order to disable ANSI colors.

!!! info

    Setup package executables are automatically code-signed during the build process if code-signing is configured in
    the InstallForge project file.

## Console Message Types

The CLI builder outputs messages to the console to inform the consumer about the current build status or any
warnings/errors. Each message has a type that is indicated by a prefix:

- `[inf]` Informational messages
- `[wrn]` Warning messages
- `[err]` Error messages

In case of any error message (`[err]`), the build process is aborted and the CLI returns exit code `1`. In all other
cases, the build process continues and ends finally with an of exit code `0`.

## Examples

Build using the setup package executable (output) file path the defined in the project file:

```bat
ifbuildx86.exe -i "MyProject.ifp"
```

Build and override the output path:

```bat
ifbuildx86.exe -i "MyProject.ifp" -o ".\dist\MyApp-Inst.exe"
```

Disable ANSI colors in the console output (useful when building a CD pipeline)

```bat
ifbuildx86.exe -i "MyProject.ifp" -o ".\dist\MyApp-Inst.exe" --no-color
```
