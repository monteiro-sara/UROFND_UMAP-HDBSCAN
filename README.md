# 3D UMAP & HDBSCAN Clustering for Clinical Samples

[![CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg?style=flat-square)](https://creativecommons.org/licenses/by/4.0/)
[![UMAP](https://img.shields.io/badge/UMAP-3D-7B61FF?style=flat-square)](https://umap-learn.readthedocs.io/en/latest/)
[![HDBSCAN](https://img.shields.io/badge/HDBSCAN-Clustering-20C9C3?style=flat-square)](https://hdbscan.readthedocs.io/en/latest/index.html)


This repository accompanies the study **“Towards a Multidimensional Exploration of Functional Neurological Disorder.”** It provides a transparent, self-contained notebook for estimating a three-dimensional UMAP embedding, identifying density-based profiles with HDBSCAN, summarizing cluster assignments, creating a publication-quality 3D figure, and exporting the resulting data and model settings.

The workflow is intended to support reproducibility and methodological reuse. It does not distribute participant-level data and should only be run with appropriately authorized, de-identified inputs.

## Project directory

This repository belongs to the broader [UROFND project directory](https://github.com/UROFND-repo), where related code, documentation, and research outputs can be collected.


## Quick start

1. Open `UROFND_UMAP+HDBSCAN.ipynb` in JupyterLab, Jupyter Notebook, VS Code, or another compatible environment.
2. Run the installation and import cells.
3. Place a de-identified delimited table at the configured input path, or change `INPUT_FILE`.
4. Replace the placeholder values in `FEATURES` with the required numeric column names.
5. Confirm the delimiter, missing-data policy, UMAP parameters, and HDBSCAN parameters.
6. Run the remaining cells in order.

The notebook uses `StandardScaler` and Euclidean distance. Alternative transformations, scalers, encodings, or distance metrics should be justified and documented rather than changed solely to improve visual separation.

## Citation

If you use or adapt this repository, please cite both the associated manuscript and the repository:

> Monteiro, S., Maillard, A., Louis, E., Hentzen, C., Al Chare, I., Baltasis, S., Teng, M., Adrien, V., & Garcin, B. (2026). *Towards a Multidimensional Exploration of Functional Neurological Disorder*. Manuscript submitted to *Neurology*.

> Monteiro, S. (2026). *URO-FND Clustering Study Repository* [Research repository]. https://github.com/UROFND-repo
