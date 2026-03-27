# Repository Layout

The Navigo repository is organized so the package, tutorial workspace, and website source stay together.

## Top-Level Structure

- `navigo/`: installable Python package code.
- Repository root: Sphinx/MyST source for the documentation website.
- `tutorials/`: unified tutorial notebooks, helper resources, and outputs.
- `data/`: centralized tutorial datasets, CSV/JSON inputs, and reference tables.
- `checkpoints/`: centralized tutorial model checkpoints.
- `submission/`: submission-oriented entrypoints and helper scripts.

## Tutorial Source Of Truth

The repository keeps a single in-repo tutorial tree under `tutorials/`.

- `tutorials/notebooks/` contains the notebooks rendered on the documentation website.
- `data/` and `checkpoints/` centralize the inputs used across tutorial sections.
- `tutorials/resources/` stores helper scripts and legacy support files still needed by some notebooks.
- `tutorials/outputs/` stores generated tutorial outputs.

## What Was Removed From The Old Split Layout

- The old embedded `dynamo/` source tree from the previous docs repository.
- Local documentation build output in `_build/`.
- Local virtual-environment files and Git metadata from the old docs folder.
- Cache directories such as `__pycache__/`.
- The duplicate root-level `tutorials/` tree was moved out of the repo to `../tutorial_backup_navigo`.
