# Polislite

A lightweight Pol.is-like.

## Setup

    - [Install][install-uv] `uv` Python package manager

   [install-uv]: https://docs.astral.sh/uv/getting-started/installation/

## Usage

This repo can be run as a self-contained example script, or used as a library.

### As A Library

This package can be installed as a library in another Python project using any package manager.

    pip install git+https://github.com/patcon/polislite.git@python-package

    uv add git+https://github.com/patcon/polislite.git@python-package

This also makes it simple to use in a Jupyter Notebook.

See sample notebook: [`polislite_library_usage.ipynb`][ipynb-example]

   [ipynb-example]: /polislite_library_usage.ipynb

### Example script

    uv run python polislite/polislite.py

### Development

Run `make` to see shortcut tasks for working on this project.

<details><summary>Output</summary>

    Consensus Statements:
    - Climate change requires immediate action (strong agreement)

    Divisive Statements:
    - Nuclear power is necessary for clean energy
    - Carbon tax should be implemented globally
    - Individual actions matter for sustainability
    - Companies should be held liable for emissions

    Group Positions:

    Group 1 characteristics:
    - strongly agrees with: Climate change requires immediate action
    - strongly agrees with: Nuclear power is necessary for clean energy
    - strongly disagrees with: Carbon tax should be implemented globally
    - strongly disagrees with: Individual actions matter for sustainability
    - strongly disagrees with: Companies should be held liable for emissions

    Group 2 characteristics:
    - strongly agrees with: Climate change requires immediate action
    - strongly agrees with: Nuclear power is necessary for clean energy
    - strongly agrees with: Carbon tax should be implemented globally
    - strongly disagrees with: Individual actions matter for sustainability
    - strongly agrees with: Companies should be held liable for emissions

    Group 3 characteristics:
    - strongly agrees with: Climate change requires immediate action
    - strongly disagrees with: Nuclear power is necessary for clean energy
    - strongly agrees with: Carbon tax should be implemented globally
    - strongly agrees with: Individual actions matter for sustainability
    - strongly agrees with: Companies should be held liable for emissions
</details>

## Status

I focused on small incremental improvements through separation of concerns.
In the branch `extract-data-and-output-rendering-to-files`, I separated the
data handling and output rendering. Subsequently, in the branch `extract-lib`,
I isolated the core algorithm into a dedicated library file.

The full changes can be reviewed in the associated pull requests.

I prefer small steps and improving abstraction before focusing more on
feature completeness for the algorithm.
