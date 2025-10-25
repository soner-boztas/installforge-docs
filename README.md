# InstallForge Docs

## Overview

This repository contains the source files for the official documentation of InstallForge.

The rendered documentation is hosted on GitHub Pages and is accessible through this URI: https://docs.installforge.net

## Contributing

Any contributions to the InstallForge documentation are highly appreciated.
Please use the _fork and pull request_ pattern for this intention.

## Setting up the Development Environment

In order to work on the documentation, you will first need to set up the development environment on your local machine.
We use [MkDocs](https://www.mkdocs.org/) for the documentation, [Poetry](https://python-poetry.org/) for dependency
management and [Poe the Poet](https://poethepoet.natn.io/index.html). As a consequence, you need to have Python version
`3.12+` installed as a prerequisite[^1]. As for Poetry, you are encouraged to install it via *pipx*
(`$ pipx install poetry`). Finally, you will need to set up your Poetry environment; follow these steps:

1. Clone this repository to the file system of your local machine.
2. Switch (`cd`) to the repository root folder (this is where the file `pyproject.toml` file resides).
3. Execute the command-line `poetry install` in your shell. This will create a Python virtual environment inside the
   repository root folder and install all dependencies into it (such as MkDocs).
4. Activate the virtual environment via `poetry env activate`. 
5. Execute the command-line `poe docs view` in order to spawn a development web server for previewing any
   changes to the documentation source files.

---

Author: Soner Boztas

[^1]: Any Python distribution such as CPython, Anaconda or Miniforge is fine. However, we recommend CPython: https://python.org.
