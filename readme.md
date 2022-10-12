# Paleo-physiography reconstruction for the Phanerozoic

## Dataset via HydroShare

Paleo-physiography reconstruction for the Phanerozoic are available from HydroShare.

Salles, T., L. Husson, M. Lorcery, B. Halder Boggiani (2022). Paleo-Physiography Elevation-only Dataset, HydroShare, http://www.hydroshare.org/resource/b3f1e3581d174bf58b00ba5672604710

## Installation

A series of recipes based on Jupyter Notebooks are available to analyse the dataset.
The easiest way to run these notebooks is through Anaconda. Once installed, open a terminal and create the environment

```bash
conda env create -f environment.yml
```

Once all the required libraries are installed, launch the environment and jupyter:

```bash
conda activate paleophysio
jupyter notebook
```

## Available notebooks

We provide 4 notebooks to get you going. The first two allow you to directly query the dataset from the HydroShare THREDDS Data Service.
This will give you a quick overview of what the information contains in the netcdf file (but will be quite limited due to the data size).

1. `hs-paleoElevation-access.ipynb`: plotting for a given time interval the elevation at global and local scale
2. `hs-paleoPhysio-access.ipynb`: plotting physiographic information at local scale

