# WaterTAP-SETO

Welcome to the code repository for **WaterTAP-SETO**!

![GitHub issues](https://img.shields.io/github/issues/watertap-org/watertap-seto)
![GitHub pull requests](https://img.shields.io/github/issues-pr/watertap-org/watertap-seto)
![CI status](https://img.shields.io/github/workflow/status/watertap-org/watertap-seto/Checks)

## Getting started (for Contributors)

**WaterTAP-SETO** supports Python versions 3.8 through 3.10.

### Prerequisites

- The conda package and environment manager, for example by using the [Miniconda installer](https://docs.conda.io/en/latest/miniconda.html#miniconda) following the steps appropriate for your operating system

### Installation

To install **WaterTAP-SETO**, run:

```sh
git clone https://github.com/watertap-org/watertap-seto && cd watertap-seto
conda create --yes --name watertap-seto-dev-env python=3.10 && conda activate watertap-seto-dev-env
pip install -r requirements-dev.txt
```

### Running tests

```sh
conda activate watertap-seto-dev-env
pytest --pyargs watertap_contrib.seto
```

### Formatting code

Before committing, the Python code must be formatted with [Black](https://black.readthedocs.io).

Black is installed by default as part of the developer dependencies. To format the code, run the following command from the local repository root directory:

```sh
conda activate watertap-seto-dev-env
black .
```
