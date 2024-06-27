# seismogen

[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![Tests status][tests-badge]][tests-link]
[![Linting status][linting-badge]][linting-link]
[![Documentation status][documentation-badge]][documentation-link]
[![License][license-badge]](./LICENSE.md)

<!--
[![PyPI version][pypi-version]][pypi-link]
[![Conda-Forge][conda-badge]][conda-link]
[![PyPI platforms][pypi-platforms]][pypi-link]
-->

<!-- prettier-ignore-start -->
[tests-badge]:              https://github.com/UCL-ARC/seismogen/actions/workflows/tests.yml/badge.svg
[tests-link]:               https://github.com/UCL-ARC/seismogen/actions/workflows/tests.yml
[linting-badge]:            https://github.com/UCL-ARC/seismogen/actions/workflows/linting.yml/badge.svg
[linting-link]:             https://github.com/UCL-ARC/seismogen/actions/workflows/linting.yml
[documentation-badge]:      https://github.com/UCL-ARC/seismogen/actions/workflows/docs.yml/badge.svg
[documentation-link]:       https://github.com/UCL-ARC/seismogen/actions/workflows/docs.yml
[conda-badge]:              https://img.shields.io/conda/vn/conda-forge/seismogen
[conda-link]:               https://github.com/conda-forge/seismogen-feedstock
[pypi-link]:                https://pypi.org/project/seismogen/
[pypi-platforms]:           https://img.shields.io/pypi/pyversions/seismogen
[pypi-version]:             https://img.shields.io/pypi/v/seismogen
[license-badge]:            https://img.shields.io/badge/License-MIT-yellow.svg
<!-- prettier-ignore-end -->

A Python package for earthquake generation.

This project is developed in collaboration with the [Centre for Advanced Research Computing](https://ucl.ac.uk/arc), University College London.

## About

### Project team

- Devaraj Gopinathan ([Devaraj-G](https://github.com/Devaraj-G))
- Dimitra Salmanidou ([dimitrasal][https://github.com/dimitrasal])
- Matt Graham ([matt-graham](https://github.com/matt-graham))

## Getting started

### Pre-requisites

<!-- Any tools or versions of languages needed to run code. For example specific Python or Node versions. Minimum hardware requirements also go here. -->

`seismogen` requires Python 3.10&ndash;3.12.

### Installation

<!-- How to build or install the application. -->

We recommend installing in a project specific virtual environment created using a environment management tool such as [Conda](https://docs.conda.io/projects/conda/en/stable/).
To install the latest development version of `seismogen` using `pip` in the currently active environment run

```sh
pip install git+https://github.com/UCL-ARC/seismogen.git
```

Alternatively create a local clone of the repository with

```sh
git clone https://github.com/UCL-ARC/seismogen.git
```

and then install in editable mode by running

```sh
pip install -e .
```

### Running tests

<!-- How to run tests on your local system. -->

Tests can be run across all compatible Python versions in isolated environments using [`tox`](https://tox.wiki/en/latest/) by running

```sh
tox
```

To run tests manually in a Python environment with `pytest` installed run

```sh
pytest tests
```

again from the root of the repository.

### Building documentation

The MkDocs HTML documentation can be built locally by running

```sh
tox -e docs
```

from the root of the repository. The built documentation will be written to
`site`.

Alternatively to build and preview the documentation locally, in a Python environment with the optional `docs` dependencies installed, run

```sh
mkdocs serve
```
