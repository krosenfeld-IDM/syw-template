# README 

An open source scientific article created using the [showyourwork](https://github.com/showyourwork/showyourwork) workflow.

# Usage

To enable the github action workflow enable read/write permissions via `Settings` -> `Actions` -> `general` -> `Workflow permission`.

## Installation of conda environment

1. Set conda `channel_priority` to `strict`"
```
conda config --set channel_priority strict
```
2. Install mamba environment:
```bash
mamba env create -f environment.yml --prefix ./env
```

If you change the `environment.yml` file you can clean and update the local environment:
```bash
mamba env update --prefix ./env --file environment.yml  --prune
```

## Build the pdf

```bash
showyourwork build --conda-frontend=mamba
```

## Remote notebook

```bash
jupyter notebook --no-browser --port=8889
```