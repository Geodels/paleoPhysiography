# Paleo-physiography reconstruction for the Phanerozoic

Example of variables available from the dataset
![Screen Shot 2022-10-12 at 4 25 39 pm](https://user-images.githubusercontent.com/7201912/195257227-c6897c9b-793a-4d30-b0d8-4b367afe7174.png)

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

The second two notebooks assume that you have downloaded the physiographic dataset locally. In addition, to evaluate some of the physiographic variables against Phanerozoic Earth database additional files (`csv`) are provided in the `dataset` folder. These notebooks:

1. `globalTrends.ipynb`: extract several of the physiographic dataset variables and plot their trends and correlations over time.
2. `wsFlux.ipynb`: analyse river discharge and sediment flux for individual basins at global scale and over time.

## Additional visualisation

The `videos` folder provides animation of global Pharenozoic elevation and river network (`topo.mp4`) and erosion/deposition rates (`ero.mp4`). It also contains a state file (`paraview_state.pvsm`) that can be loaded in Paraview to visualise individual netcdf file in 3D. 

