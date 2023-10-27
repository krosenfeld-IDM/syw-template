# README 

An open source scientific article created using the [showyourwork](https://github.com/showyourwork/showyourwork) workflow.

# Usage

## Installation

Install mamba environment:
```bash
mamba env create -f environment.yml --prefix ./env
```
Clean and update the environment:
```bash
mamba env update --prefix ./env --file environment.yml  --prune
```

## Build

```bash
showyourwork build --conda-frontend=mamba
```

## Remote notebook

```bash
jupyter notebook --no-browser --port=8889
```