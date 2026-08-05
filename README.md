# Workshop: 2D Deep Learning Segmentation

This repository contains materials for a workshop on 2D cell segmentation using deep learning tools, specifically **Cellpose** and **StarDist** with **Napari** visualization.

## Prerequisites

Install [Pixi](https://pixi.sh) - a fast, cross-platform package manager built on conda-forge:

- **Installation guide**: [https://pixi.sh/latest/#installation](https://pixi.sh/latest/#installation)
- Quick install (Unix/macOS):
  ```bash
  curl -fsSL https://pixi.sh/install.sh | bash
  ```
- Quick install (Windows PowerShell):
  ```powershell
  iwr -useb https://pixi.sh/install.ps1 | iex
  ```

## Getting Started

### Clone this repository

```bash
git clone https://github.com/acorbat/workshop_3d_dl_segmentation.git
cd workshop_2d_dl_segmentation
```

### In a terminal in the workshop notebook
### Install the environment

```bash
pixi run setup
```

This will set up the environments with Python and all required packages (napari, bioio, cellpose, stardist) and download `Tissue_16x_avg.nd2` and `Nuclei_avg16x.nd2` (a 2D microscopy images) from Zenodo to the `data/` folder.

### Run Deep Learnings models for analysis

#### Cellpose

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/IgnacioSallaberry/workshop_2D_segmentation/blob/main/notebooks/cellpose_napari_2d.ipynb)


```bash
pixi run cellpose
```
Select the cellpose environment by scrolling with the arrows

```bash
  default
> cellpose
  cellpose-cpu
  stardist
```

You can also test your images in [HuggingFace Spaces](https://huggingface.co/spaces/mouseland/cellpose)

#### Stardist

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/IgnacioSallaberry/workshop_2D_segmentation/blob/main/notebooks/stardist_napari_2d.ipynb)

```bash
pixi run stardist
```
Select the stardist environment by scrolling with the arrows

```bash
  default
  cellpose
  cellpose-cpu
> stardist
```
Or open them in VS Code with the Jupyter extension.

## Workshop Guide

For a detailed walkthrough of the notebooks and additional learning resources, see the [**workshop.md**](workshop.md) file. It includes:
- Step-by-step instructions for each notebook
- Learning objectives
- Tips for success
- Information about testing additional models on BioImage.io

## Environment Details

- **Python**: 3.11 (required for StarDist compatibility)
- **Key packages**: napari, bioio, cellpose, stardist
- **Platforms**: Windows, Linux

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
