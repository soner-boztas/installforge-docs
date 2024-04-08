# Using Predefined Constants

## Introduction

InstallForge supports various predefined constants enclosed in `<` `>` characters. These constants are validated by the
native setup engine during runtime and can be used to increase the flexibility of your setup packages.

!!! info

    All predefined constant names are case-insensitive.

In InstallForge constants are divided into the following two groups:

### Setup Constants

Setup constants contain specific information provided by the user when creating a setup package as well as data entered
by the end-user when running a setup.

!!! info

    One exception is the `<InstallPath>` constant which contains the installation path selected by the user on the
    `Select Application Folder` dialog of the setup. This constant belongs to the _Path Constants_ group.

### Path Constants

Path constants can be used to determine the path of a
Windows [special/shell folder](https://en.wikipedia.org/wiki/Special_folder) on the target machine during runtime.

## Setup Constants

The following table lists the supported setup constants.

{{ read_csv('../../data/SetupConstants.csv') }}

## Path Constants

!!! info

    Paths provided by the `Path Constants` do not include an appending backslash.

!!! danger "Important"

    Setup packages created with InstallForge usually require administrator privileges. If you remove this configuration and the user running your setup package does not have elevated rights, changes in per-machine folders will not be possible.

{{ read_csv('../../data/PathConstants.csv') }}
