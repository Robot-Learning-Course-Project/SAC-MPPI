# Soft Actor Critique Model Predictive Path Integral

[![pre-commit](https://github.com/Robot-Learning-Course-Project/SAC-MPPI/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/Robot-Learning-Course-Project/SAC-MPPI/actions/workflows/pre-commit.yml)

## Installation

1. Clone the repository

   ```Shell
   git clone --recursive git@github.com:Robot-Learning-Course-Project/SAC-MPPI.git
   ```

1. Create an environment, either using conda or virtualenv

   1. Using conda

      ```Shell
      cd SAC-MPPI
      conda env create -f environment.yml
      conda activate sac-mppi
      pip install -e .

      cd sac_mppi/dial_mpc
      pip install -e .

      cd ../rsl_rl
      pip install -e .
      ```

   1. Using virtualenv

      ```Shell
      python3 -m venv .venv
      source .venv/bin/activate
      pip install -e .
      ```

1. Run example:

   ```Shell
   sac-mppi -c ./config/default.yaml
   ```

## Developer Quick Start

- Run [scripts/dev-setup.sh](scripts/dev-setup.sh) to setup the development environment
