# Installation

## Package install

Install the Navigo package from the main code repository, not from this documentation repository.

```bash
git clone <your-github-url> Navigo-release
cd Navigo-release
pip install -r requirements.txt
pip install -e .
```

## Build the documentation locally

```bash
pip install -r requirements.txt
sphinx-build -b html . _build/html
```

## Repository notes

- This repository contains the standalone documentation website.
- Tutorial notebooks live in `tutorials/`.
- Runtime data and checkpoints are expected from the main `Navigo-release` workspace.
